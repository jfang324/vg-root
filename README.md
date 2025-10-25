## About The Project

This is the root directory of the [ValoGraphs](https://valographs.com) project, a data visualization platform for Valorant performance data.

## Project Structure

-   [vg-frontend](https://github.com/jfang324/vg-frontend) - Next.js + shadcn/ui based user interface for ValoGraphs
-   [vg-backend](https://github.com/jfang324/vg-backend) - NestJS based REST API for ValoGraphs
-   [vg-deploy](https://github.com/jfang324/vg-deploy) - Bash scripts for provisioning and deploying ValoGraphs on a fresh VMmachine

## Getting Started

To have the entire project running locally, follow these steps:

1. Clone the backend repository and install dependencies:

```bash
git clone https://github.com/jfang324/vg-backend.git
cd vg-backend
npm install
```

2. Run the database migrations if you are using a new database:

```bash
npx supabase db push
```

3. Generate the API clients and Supabase types:

```bash
npm run generate-api-clients
npm run generate-supabase-types
```

4. Start the backend server:

```bash
npm run start:dev
```

5. Clone the frontend repository and install dependencies:

```bash
git clone https://github.com/jfang324/vg-frontend.git
cd vg-frontend
npm install
```

6. Start the frontend server:

```bash
npm run dev
```

Now if you've followed the README instructions for setting up the `.env` files for each component, you should have the entire project running locally.

## Tools & Technologies

-   **Frontend:** Next.js (App Router), shadcn/ui, Tailwind CSS, React
-   **Backend:** NestJS, Supabase (PostgreSQL), Redis, Node.js
-   **Infrastructure:** Route 53, EC2, Docker (Docker Compose), Caddy, Vercel
-   **Common:** TypeScript, Jest, GitHub Actions, Swagger, ESLint, OpenAPI Generator

## Links

-   **Production:** [ValoGraphs](https://valographs.com)
-   **API Docs:** [api.valographs.com/swagger](https://api.valographs.com/swagger)
-   **OpenAPI Spec:** [swagger.yaml](https://api.valographs.com/swagger.yaml)
