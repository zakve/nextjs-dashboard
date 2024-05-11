## Next.js App Router Dashboard

### Install and Run
```
git clone https://github.com/zakve/nextjs-dashboard.git
cd nextjs-dashboard
npm i
npm run dev
```

For init DB run
```
// see .env.example first
npm run seed
``` 

### Stack and features
- NextJS 14
- Styles - Tailwind 
- Image and fonts optimization
- Routing (App router)
- Data fetching (Static, Dynamic, Prerendering)
- Vercel Database
- Search and pagination
- Mutating data
- Error handling (general + 404)
- Form validation
- Authentication
- Metadata

### Summary
To recap, you've done a few things to optimize data fetching in your application, you've:

1. Created a database in the same region as your application code to reduce latency between your server and database.
2. Fetched data on the server with React Server Components. This allows you to keep expensive data fetches and logic on the server, reduces the client-side JavaScript bundle, and prevents your database secrets from being exposed to the client.
3. Used SQL to only fetch the data you needed, reducing the amount of data transferred for each request and the amount of JavaScript needed to transform the data in-memory.
4. Parallelize data fetching with JavaScript - where it made sense to do so.
5. Implemented Streaming to prevent slow data requests from blocking your whole page, and to allow the user to start interacting with the UI without waiting for everything to load.
6. Move data fetching down to the components that need it, thus isolating which parts of your routes should be dynamic in preparation for Partial Prerendering.


For more information, see the [course curriculum](https://nextjs.org/learn) on the Next.js Website.
