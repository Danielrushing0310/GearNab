# GearNab
import React from 'react';
import './HomePage.css';
import FeaturedListingCard from './components/FeaturedListingCard';
import SearchBar from './components/SearchBar';
import PlatformButtons from './components/PlatformButtons';

const HomePage = () => {
  return (
    <div className="homepage">
      <header className="hero-section">
        <h1>GearNab</h1>
        <p className="slogan">Find it. Nab it. Play on.</p>
        <SearchBar />
      </header>

      <section className="featured-listings">
        <h2>Featured Gear</h2>
        <div className="listing-grid">
          <FeaturedListingCard title="Fender Stratocaster" price="$899" location="Nashville, TN" />
          <FeaturedListingCard title="Yamaha Stage Custom" price="$499" location="Austin, TX" />
          <FeaturedListingCard title="Moog Sub Phatty" price="$850" location="Portland, OR" />
        </div>
      </section>

      <section className="platform-search">
        <h2>Search Other Platforms</h2>
        <PlatformButtons />
      </section>
    </div>
  );
};

export default HomePage;
