# Architecture Case Studies — J.M. Eahsan

I'm Jamal Mostafa Eahsan (J.M.), a Full Stack Developer & System Architect and Software Engineer L4 at Codezzi Systems LLC in Dhaka, Bangladesh. I work across the whole stack, from React and Next.js frontends to Node.js and NestJS APIs on PostgreSQL, and I care most about the decisions underneath: data boundaries, failure handling and keeping systems simple as they grow.

This repository explains how two recent production systems are put together: the problem, my role, the architecture, and the design decisions I made with their trade-offs.

- LinkedIn: https://www.linkedin.com/in/jamalmostafaeahsan/
- Portfolio: https://my-portfolio-v2-one-ashy.vercel.app/

---

## Case studies

### [Hiring Manager](./hiring-manager/README.md)
**Multi-tenant hiring platform (ATS)** · Next.js · NestJS · Prisma · PostgreSQL

A SaaS platform where each company runs its own hiring: positions, a configurable drag-and-drop pipeline, candidates, interviews, a talent pool and bulk email sent from the company's own mailbox. A super admin portal manages the companies. I built most of it with one teammate in about 12 days.

Covers: tenant isolation, a pipeline modelled as data, role-based access, and a safe-to-retry scheduled bulk email engine.

### [Sky Chat](./sky-chat/README.md)
**Real-time contact-centre live chat** for a client · React · TypeScript · Socket.IO · Redux Toolkit

A live-chat platform with a customer chat widget, an agent console and an admin dashboard. I was the only frontend developer and built all of the client applications.

Covers: Socket.IO messaging with authenticated agent connections, optimistic sends, reconnect and room rejoin, and a polling fallback when the realtime connection drops.

---

Source code is private (client and company work); this repository documents architecture only.
