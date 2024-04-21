# graphql

### What is graphQL
- graph query language
- data is represented as graph
- all graphql calls by default are HTTP POST call
- ![image](https://github.com/rhythm55/graphql/assets/36883992/d2b09396-d8c6-469b-95a8-6a4e3f21bc47)

### Why graphql
- avoid over-fetching : can fetch selective data. ex: we have 10 fields and we just want to fetch topArtist.
- avoid under-fetching
    - to fetch topArtist, topAlbum etc we need to make seprate API calls. Using graphQL in one api call only we can fetch both.
- Better mobile performance
  - mobiles dont have hardware and ram like desktops. fetching is a costly operation. with graphql we can limit data to be loaded on mobile and on desktop.
- Efficiency and precision
- Declarative data fetching
- Hierarichal structure
- Strongly typed
    - ![Screenshot 2024-04-21 at 4 58 57 PM](https://github.com/rhythm55/graphql/assets/36883992/b748538b-266e-46a3-9e88-3799602b27ef)
- Introspection - documentation is available
    - ![Screenshot 2024-04-21 at 4 59 20 PM](https://github.com/rhythm55/graphql/assets/36883992/293e824f-3c17-409a-907c-9f4cc58d3807)
- Real time capabilities subscription

### Rest VS graphQL

Aspect | #Rest | #GraphQL
--- | --- | ---
Data fetching | Multiple endpoint | Single Endpoint
Request structure | Fixed structure + HTTP methods | Flexible (Query + Mutation)
Over fetching / Under fetching | Issue | Resolved
Response Size | fixed | flexible
Versioning | Explicit versioning | Flexible (can depricate the field in existing one)
Schema Definition | Not well defined | explicit Schema Definition
Real time capabilities | web sockets | subscription
Tooling support | postman | playground
Caching | Relies on HTTP cache | Fine Grained - apollo client provides it
Client control | no | Yes
