# Flashcards — quick Q/A for interview review

Q: What are the main HTTP methods and when to use them?
A: GET (read), POST (create), PUT (replace), PATCH (partial update), DELETE (remove).

Q: What is CORS and why is it needed?
A: Cross-Origin Resource Sharing — browser security policy that allows controlled access to resources from another origin; configured via server response headers.

Q: REST vs GraphQL vs tRPC — quick differences?
A: REST: resource-based endpoints. GraphQL: typed query language; single endpoint with flexible queries. tRPC: typesafe RPC for TypeScript enabling end-to-end type safety without GraphQL schema.

Q: JWT vs session-based auth?
A: JWT: stateless tokens (client stores token), sessions: server stores session state. JWTs avoid server-state but require careful handling (revocation, expiration).

Q: What is Caching and where to put it?
A: Cache reduces latency: browser cache, CDN (edge), in-memory (Redis), application-level caching (memoization). Use CDN for static assets and Redis for fast data caching.

Q: SQL index basics?
A: Indexes speed lookups (B-tree common). Indexes slow writes and take space. Index primary keys, foreign keys, and columns used in WHERE/order by.

Q: TypeScript: difference between type and interface?
A: Both define shapes. interface supports declaration merging; type is more flexible (unions, mapped types).

Q: Next.js: difference SSR, SSG, ISR?
A: SSR: server renders per request. SSG: static at build time. ISR: incremental static regeneration — static pages updated at runtime.

Q: Prisma: how to run migrations?
A: `npx prisma migrate dev` (dev), `npx prisma db push` (schemaless push), and manage schema.prisma file.

Q: How to secure passwords?
A: Hash with a slow algorithm (bcrypt, argon2), never store plaintext, add proper salt (bcrypt includes salt).

Q: What is a reverse proxy?
A: A server that forwards client requests to backend services (e.g., Nginx, Envoy). Useful for TLS termination, load balancing, and routing.

Q: What’s the CAP theorem?
A: In distributed systems, you can only have two of: Consistency, Availability, Partition tolerance.

Q: How to prevent SQL injection?
A: Use parameterized queries/ORMs and input validation, never concatenate SQL strings with user input.

Q: What is a content delivery network (CDN) used for?
A: Distribute static assets geographically to reduce latency and offload origin servers.

Q: One-liner for explaining Prisma?
A: Prisma is a type-safe ORM for Node/TypeScript that generates a client from your schema and simplifies DB access with compile-time types.
