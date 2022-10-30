# Fullstack Authentication Example with Next.js and NextAuth.js

This is the starter project for the fullstack tutorial with Next.js and Prisma. You can find the final version of this project in the [`final`](https://github.com/prisma/blogr-nextjs-prisma/tree/final) branch of this repo.

// the pages/index.tsx works on dev server, but only fetch data one time on deployment server :(
// if readme.md (or probably other files' too) content is changed, the pages/index.tsx got updated 
Has the problem of Incremental Static Regeneration (ISR) with 10s interval on getStaticProps 
The page need to be reopened after the interval to purge the cache.
Probably working solution is to change the ISR to ISR On-Demand, or to change the getStaticProps to getServerSideProps
