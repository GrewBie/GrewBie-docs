# Table of contents

##   👋 Introduction
    *   [Welcome](./README.md)
    *   [Project Overview: Grewbie_v2](./introduction/project-overview.md) (SaaS for visual workflow automation, target audience)
    *   [Key Features](./introduction/key-features.md) (Workflow Editor, Automated Executions, Billing, Credentials, Analytics)
    *   [Tech Stack High-Level](./introduction/tech-stack.md) (Next.js App Router, React, TypeScript, Prisma, Stripe, Tailwind CSS, Shadcn/ui, [Auth Provider?])

##  🚀 Getting Started (For Users/Stakeholders)
    *   [Accessing Grewbie_v2](./getting-started-users/accessing.md) (Sign-up, Sign-in process)
    *   [Dashboard Overview](./getting-started-users/dashboard-overview.md)
    *   [Creating Your First Workflow](./getting-started-users/creating-workflow.md)
    *   [Understanding Billing & Credits](./getting-started-users/billing.md)

##  💻 Developer Setup & Onboarding
    *   [Prerequisites](./developer-guide/setup/prerequisites.md)
    *   [Cloning the Repository](./developer-guide/setup/cloning.md)
    *   [Installation](./developer-guide/setup/installation.md) (Show `package.json` scripts)
    *   [Environment Variables](./developer-guide/setup/environment-variables.md) (Need content of `.env.example` or list of vars)
    *   [Database Setup (Prisma)](./developer-guide/setup/database-setup.md) (Migrating, seeding)
    *   [Running Locally](./developer-guide/setup/running-locally.md)

##  🏗️ Architecture & Core Concepts
    *   [Project Structure Overview](./developer-guide/architecture/project-structure.md) (Explain `app`, `actions`, `components`, `lib`, `hooks`, `prisma`, `schema` etc.)
    *   [Next.js App Router Usage](./developer-guide/architecture/app-router.md)
        *   [Routing & Route Groups](./developer-guide/architecture/routing.md) (Explain `(auth)`, `(dashboard)`, `(home-landing)`)
        *   [Server Components vs. Client Components](./developer-guide/architecture/server-client-components.md) (Examples from your codebase)
        *   [Data Fetching: Server Actions & Route Handlers](./developer-guide/architecture/data-fetching.md) (Focus on `actions/` and `app/api/`)
    *   [Authentication (Clerk/Other?)](./developer-guide/architecture/authentication.md) (Explain `app/(auth)/`, `middleware.ts`)
    *   [State Management](./developer-guide/architecture/state-management.md) (`FlowValidationContext.tsx`, patterns in `AppProviders.tsx`)
    *   [Styling (Tailwind CSS & Shadcn/ui)](./developer-guide/architecture/styling.md)
    *   [Database (Prisma)](./developer-guide/architecture/database.md) (Key models from `schema.prisma`, common query patterns)
    *   [Workflow Engine Internals](./developer-guide/architecture/workflow-engine.md) (Deep dive into `lib/workflow/`, `executeWorkflow.ts`, `executor/Registry.ts` and individual executors)
    *   [Billing & Stripe Integration](./developer-guide/architecture/billing-stripe.md) (`lib/stripe/`, `app/api/webhooks/stripe/route.ts`)
    *   [Credentials Management](./developer-guide/architecture/credentials.md) (`lib/credential.ts`)
    *   [Input Validation (Zod Schemas)](./developer-guide/architecture/validation.md) (Explain `schema/` directory usage)
##   🧩 Components & Modules
    *   [UI Components (Shadcn/ui & Custom)](./developer-guide/components/ui-components.md) (Overview of `components/ui/` and `components/accernity-ui/`)
    *   [Workflow Editor Components](./developer-guide/components/workflow-editor.md) (Key components from `app/workflow/_components/` like `Editor.tsx`, `nodes/`, `edges/`, `TaskMenu.tsx`)
    *   [Dashboard Components](./developer-guide/components/dashboard-components.md) (Key components from `app/(dashbaord)/_components/`)
    *   [Server Actions (`actions/`)](./developer-guide/modules/server-actions.md) (List key actions and their purpose)
    *   [Utility Functions & Hooks (`lib/`, `hooks/`)](./developer-guide/modules/utilities-hooks.md)

##   🧪 Testing
    *   [Testing Strategy](./developer-guide/testing/strategy.md) (Do you have tests? What kind? Tools used?)

##   💅 Coding Standards & Best Practices
    *   [Code Style (ESLint, Prettier)](./developer-guide/standards/code-style.md) (From `.eslintrc.json`)
    *   [Naming Conventions](./developer-guide/standards/naming-conventions.md)
    *   [Commit Message Guidelines](./developer-guide/standards/commit-messages.md)

##   🔄 CI/CD & Deployment
    *   [Build Process](./developer-guide/deployment/build-process.md)
    *   [Deployment Platform (Vercel? Netlify?)](./developer-guide/deployment/platforms.md)
    *   [CI/CD Pipeline](./developer-guide/deployment/ci-cd.md)

##   🤝 Contributing
    *   [Branching Strategy](./developer-guide/contributing/branching-strategy.md)
    *   [Submitting Pull Requests](./developer-guide/contributing/pull-requests.md)

##   📖 API Reference
    *   [`/api/webhooks/stripe`](./api-reference/stripe-webhook.md)
    *   [`/api/workflows/cron`](./api-reference/workflow-cron.md)
    *   [`/api/workflows/execute`](./api-reference/workflow-execute.md)

##   📚 Glossary
    *   [Project-Specific Terms](./glossary.md) (Workflow, Node, Executor, Task, Credential, Execution Plan)
