# Deployment Guide

## Prerequisites

- Node.js 18+
- Cloudflare account
- Wrangler CLI installed

## Steps

1. Install dependencies: `npm install`
2. Configure environment variables (see .env.example)
3. Run database migrations: `npm run db:migrate`
4. Deploy to Cloudflare Pages: `npm run deploy`
5. Configure email routing in Cloudflare dashboard

## Environment Variables

See `.env.example` for required configuration.
