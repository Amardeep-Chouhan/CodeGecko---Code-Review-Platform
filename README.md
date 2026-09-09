# 🦎 CodeGecko

<div align="center">

### AI-Powered Code Review Platform

**Supercharge your development workflow with advanced AI-powered code reviews.**

[![Live Demo](https://img.shields.io/badge/demo-live-success)](https://coderabbit-flame.vercel.app)
[![Next.js](https://img.shields.io/badge/Next.js-16-black)](https://nextjs.org/)
[![TypeScript](https://img.shields.io/badge/TypeScript-5-blue)](https://www.typescriptlang.org/)
[![License](https://img.shields.io/badge/license-MIT-green)](LICENSE)

</div>

---

## 📋 Table of Contents

* [Overview](#-overview)
* [Features](#-features)
* [Tech Stack](#-tech-stack)
* [Getting Started](#-getting-started)
* [Project Structure](#-project-structure)
* [Development](#-development)
* [Deployment](#-deployment)
* [Contributing](#-contributing)
* [License](#-license)
* [Acknowledgments](#-acknowledgments)
* [Contact & Support](#-contact--support)

---

## 🎯 Overview

**CodeGecko** is an AI-powered code review platform designed to help development teams ship better software, faster.

It automates code reviews, identifies potential bugs and security issues, and provides actionable suggestions for improving code quality. Built with **Next.js 16** and modern web technologies, CodeGecko delivers intelligent, context-aware code analysis while streamlining the pull request review workflow.

---

## ✨ Features

* 🤖 **AI-Powered Code Reviews**
  Advanced AI analyzes code for bugs, security vulnerabilities, code quality issues, and best practices.

* ⚡ **Fast GitHub Integration**
  Seamlessly integrates with GitHub to automate pull request code reviews.

* 🔒 **Secure Authentication**
  GitHub OAuth integration provides secure and convenient authentication.

* 📊 **Detailed Analytics**
  Track code quality metrics, review activity, and review history.

* 🎨 **Modern & Responsive UI**
  Clean, responsive interface designed with modern UI principles.

* 🔄 **Real-Time Updates**
  Receive instant feedback on code changes through Inngest-powered workflows.

* 📝 **Custom Review Rules**
  Configure review rules according to your team's coding standards and requirements.

---

## 🛠 Tech Stack

### Frontend

* **[Next.js](https://nextjs.org/)** - React framework with App Router
* **[TypeScript](https://www.typescriptlang.org/)** - Type-safe JavaScript development
* **[Tailwind CSS](https://tailwindcss.com/)** - Utility-first CSS framework
* **[shadcn/ui](https://ui.shadcn.com/)** - Reusable and accessible UI components

### Backend & Database

* **[Prisma](https://www.prisma.io/)** - Type-safe ORM
* **[PostgreSQL](https://www.postgresql.org/)** - Relational database
* **[Inngest](https://www.inngest.com/)** - Background job processing and workflows

### Development & Deployment

* **[Bun](https://bun.sh/)** - JavaScript runtime and package manager
* **[ESLint](https://eslint.org/)** - Code linting
* **[Vercel](https://vercel.com/)** - Deployment platform

---

## 🚀 Getting Started

Follow the steps below to run CodeGecko locally.

### Prerequisites

Make sure you have the following installed or configured:

* [Bun](https://bun.sh/) (recommended) or Node.js 18+
* PostgreSQL database
* GitHub OAuth App credentials

### Installation

#### 1. Clone the Repository

```bash
git clone https://github.com/dndmein-rgb/CodeGecko.git
cd CodeGecko
```

#### 2. Install Dependencies

Using Bun:

```bash
bun install
```

Or using npm:

```bash
npm install
```

#### 3. Configure Environment Variables

Create a `.env` file in the project root:

```env
# Database
DATABASE_URL="postgresql://user:password@localhost:5432/codegecko"

# GitHub OAuth
GITHUB_CLIENT_ID="your_github_client_id"
GITHUB_CLIENT_SECRET="your_github_client_secret"

# Inngest
INNGEST_EVENT_KEY="your_inngest_key"

# NextAuth
NEXTAUTH_SECRET="your_nextauth_secret"
NEXTAUTH_URL="http://localhost:3000"
```

> **Note:** Replace the placeholder values with your actual credentials.

#### 4. Set Up the Database

Generate the Prisma client:

```bash
bunx prisma generate
```

Push the database schema:

```bash
bunx prisma db push
```

#### 5. Start the Development Server

Using Bun:

```bash
bun dev
```

Or using npm:

```bash
npm run dev
```

#### 6. Open the Application

Once the development server is running, open:

```text
http://localhost:3000
```

---

## 📁 Project Structure

```text
CodeGecko/
├── app/                    # Next.js application directory
│   ├── api/                # API routes
│   ├── (auth)/             # Authentication pages
│   └── (dashboard)/        # Dashboard pages
│
├── components/             # React components
│   ├── ui/                 # shadcn/ui components
│   └── ...                 # Custom components
│
├── hooks/                  # Custom React hooks
├── inngest/                # Inngest background jobs
├── lib/                    # Utility functions and configurations
├── module/                 # Business logic modules
│
├── prisma/                 # Prisma configuration and database schema
│   └── schema.prisma       # Prisma schema
│
├── public/                 # Static assets
└── ...                     # Configuration files
```

---

## 💻 Development

### Available Scripts

#### Development

Start the development server:

```bash
bun dev
```

#### Production Build

Create a production build:

```bash
bun run build
```

#### Production Server

Start the production server:

```bash
bun start
```

#### Linting

Run ESLint:

```bash
bun run lint
```

#### Formatting

Format the codebase:

```bash
bun run format
```

### Database Commands

Open Prisma Studio:

```bash
bunx prisma studio
```

Create and apply a database migration:

```bash
bunx prisma migrate dev
```

---

## 🌐 Deployment

### Deploy with Vercel

The recommended deployment platform for CodeGecko is [Vercel](https://vercel.com/).

1. Push the project to GitHub.
2. Import the repository into Vercel.
3. Configure all required environment variables.
4. Deploy the application.

[![Deploy with Vercel](https://vercel.com/button)](https://vercel.com/new/clone?repository-url=https://github.com/dndmein-rgb/CodeGecko)

### Other Deployment Platforms

CodeGecko can also be deployed to platforms that support Next.js applications, including:

* [Railway](https://railway.app/)
* [Render](https://render.com/)
* [AWS](https://aws.amazon.com/)
* [Google Cloud](https://cloud.google.com/)

---

## 🤝 Contributing

Contributions are welcome and appreciated.

Before submitting changes, please make sure to:

* Write properly typed TypeScript code.
* Follow the existing project structure and coding conventions.
* Add tests for new functionality where applicable.
* Update the documentation when necessary.
* Keep commits atomic and descriptive.

---

## 📄 License

This project is licensed under the **MIT License**.

See the [LICENSE](LICENSE) file for more information.

---

## 🙏 Acknowledgments

* Built with [Next.js](https://nextjs.org/)
* UI components powered by [shadcn/ui](https://ui.shadcn.com/)
* Inspired by modern AI-powered code review platforms

---

## 📧 Contact & Support

* **Website:** [coderabbit-flame.vercel.app](https://coderabbit-flame.vercel.app)
* **Issues:** [GitHub Issues](https://github.com/dndmein-rgb/CodeGecko/issues)
* **Discussions:** [GitHub Discussions](https://github.com/dndmein-rgb/CodeGecko/discussions)

---

<div align="center">

### ⭐ Star this repository if you find it helpful!

</div>
