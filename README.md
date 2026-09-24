# ScrapMart

Mobile-friendly scrap catalog with WhatsApp enquiry flow and PostgreSQL.

## Local setup
1. Copy `.env.example` to `.env`.
2. Fill `DATABASE_URL`, `ADMIN_EMAIL`, `ADMIN_PASSWORD`, and WhatsApp number.
3. `npm install`
4. `npx prisma generate`
5. `npx prisma db push`
6. `npx tsx prisma/seed.ts`
7. `npm run dev`

## Production
Push this repository to GitHub, import it into Vercel, add the environment variables, and deploy.

Note: the included `/admin` page is a dashboard shell. Before public production use, secure it with server-side authentication and add CRUD actions for products/settings.