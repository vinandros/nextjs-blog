# Rendering

## Static generation

### Static generation without data

For static html and css that don't required to fetch data on build time.

### Static generation with data

Fort static html and css that required to fetch data on build time.
To user this feature export this component **getStaticProps** in async way, this allow to fetch data on build time.

## Pre-rendering or server side rendering getServerSideProps

Pre-rendering is used when content change on each request depending of user interaction.
To user this feature export this component **getServerSideProps(context)** in async way, this allow to pre-render a page whose data must be fetched at request time.

## Client side rendering

This approach works well for user dashboard pages, for example. Because a dashboard is a private, user-specific page, SEO is not relevant, and the page doesn’t need to be pre-rendered. The data is frequently updated, which requires request-time data fetching.
**React hook SWR** to fetch data on client site.
