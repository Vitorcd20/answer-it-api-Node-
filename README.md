**Project developed using modern technologies
to create a robust and efficient API.**

------------------------------------------------------------------------

### 🚀 Technologies

-   **Node.js** with native TypeScript (`--experimental-strip-types`)\
-   **Fastify** -- A fast and efficient web framework\
-   **PostgreSQL** with **pgvector** extension for vector support\
-   **Drizzle ORM** -- Type-safe database operations\
-   **Zod** -- Schema validation\
-   **Docker** -- Database containerization

------------------------------------------------------------------------

### 🏗️ Architecture

The project follows a modular architecture with:\
- Clear separation of concerns between routes, schemas, and database
connection\
- Schema validation using Zod for type safety\
- Type-safe ORM operations using Drizzle\
- Centralized environment variable validation

------------------------------------------------------------------------

### ⚙️ Setup and Configuration

#### **Prerequisites**

-   Node.js (version with support for `--experimental-strip-types`)\
-   Docker and Docker Compose

#### **1. Clone the repository**

``` bash
git clone <repository-url>
cd server
```

#### **2. Set up the database**

``` bash
docker-compose up -d
```

#### **3. Configure environment variables**

Create a `.env` file in the project root with:

    PORT=3333
    DATABASE_URL=postgresql://docker:docker@localhost:5432/answer

#### **4. Install dependencies**

``` bash
npm install
```

#### **5. Run database migrations**

``` bash
npx drizzle-kit migrate
```

#### **6. (Optional) Seed the database with sample data**

``` bash
npm run db:seed
```

#### **7. Run the project**

**Development:**

``` bash
npm run dev
```

**Production:**

``` bash
npm start
```

------------------------------------------------------------------------

### 📚 Available Scripts

-   `npm run dev` -- Runs the server in development mode with hot
    reload\
-   `npm start` -- Runs the server in production mode\
-   `npm run db:seed` -- Seeds the database with sample data

------------------------------------------------------------------------

### 🌐 Endpoints

The API will be available at: <http://localhost:3333>

-   **GET /health** -- Application health check\
-   **GET /rooms** -- List available rooms
