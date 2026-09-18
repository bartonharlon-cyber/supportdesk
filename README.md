# SupportDesk

A full stack customer support ticketing platform built to showcase end-to-end product development — from database design to a live, real-time UI. Designed and built solo by James Onuoha.

## Why this project

After 10+ years doing full stack development and technical support work for clients, SupportDesk combines both: it's the kind of internal tool a growing company would actually use to manage customer issues, and it's built to demonstrate production-grade full stack skills in one place — auth, roles, real-time data, a relational schema, and a clean dashboard UI.

## Features

- **Ticket management** — create, assign, prioritize, tag, and resolve support tickets
- **Role-based access control** — separate views/permissions for Admin, Agent, and Customer roles
- **Real-time updates** — ticket status and new replies update live via WebSockets, no page refresh
- **Analytics dashboard** — response time, resolution time, ticket volume by category, agent performance
- **Search & filtering** — filter tickets by status, priority, assignee, and date range
- **Email notifications** — ticket updates trigger notifications to the relevant user
- **Audit trail** — every status change and assignment is logged per ticket

## Tech stack

| Layer | Technology |
|---|---|
| Frontend | React, TypeScript, Tailwind CSS |
| Backend | Node.js, Express |
| Database | PostgreSQL |
| Real-time | Socket.IO |
| Auth | JWT with refresh tokens |
| Deployment | Docker, deployable to any cloud VM or PaaS |

## Project structure

```
supportdesk/
├── client/              # React frontend
│   ├── src/
│   │   ├── components/
│   │   ├── pages/
│   │   ├── hooks/
│   │   └── api/
│   └── package.json
├── server/              # Express backend
│   ├── src/
│   │   ├── routes/
│   │   ├── controllers/
│   │   ├── models/
│   │   ├── middleware/
│   │   └── sockets/
│   └── package.json
├── docs/
│   └── schema.md        # Database schema reference
├── docker-compose.yml
└── README.md
```

## Roadmap

- [ ] Project scaffolding (client + server + DB schema)
- [ ] Auth (signup/login, JWT, roles)
- [ ] Ticket CRUD + assignment logic
- [ ] Real-time updates via Socket.IO
- [ ] Analytics dashboard
- [ ] Email notifications
- [ ] Docker deployment setup
- [ ] Seed data + demo mode for portfolio viewers

## Getting started

```bash
# clone the repo
git clone https://github.com/bartonharlon-cyber/supportdesk.git
cd supportdesk

# install dependencies (once scaffolding is added)
cd client && npm install
cd ../server && npm install

# run with docker-compose (once added)
docker-compose up
```

## About

Built by James Onuoha, full stack developer (10+ years, remote/freelance). Open to remote full stack roles.
