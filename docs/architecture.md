# Architecture Overview

## Project Structure

MoEmail is a Cloudflare-based email service built with Next.js and Drizzle ORM.

### Core Components

- **app/** - Next.js App Router pages and API routes
- **workers/** - Cloudflare Workers for email processing
- **drizzle/** - Database schema and migrations
- **packages/** - Shared utility packages

### Data Flow

1. Incoming email → Cloudflare Email Worker → D1 database
2. User requests → Next.js API → D1 database
3. Authentication → Middleware → Session validation

## Deployment

The application is deployed on Cloudflare Pages with Workers for email handling.
