# 💰 AI Finance - Smart Personal Finance Manager

> Your AI-powered companion for intelligent financial management and insights

[![Next.js](https://img.shields.io/badge/Next.js-15-black?style=flat-square&logo=next.js)](https://nextjs.org/)
[![TypeScript](https://img.shields.io/badge/TypeScript-5.0-blue?style=flat-square&logo=typescript)](https://www.typescriptlang.org/)
[![License](https://img.shields.io/badge/License-MIT-green?style=flat-square)](LICENSE)

---

## 📋 Table of Contents

- [Problem Statement](#-problem-statement)
- [Solution](#-solution)
- [Features](#-features)
- [Tech Stack](#-tech-stack)
- [Tools Used](#-tools-used)
- [Getting Started](#-getting-started)
- [Environment Variables](#-environment-variables)
- [Future Scope](#-future-scope)
- [Contributing](#-contributing)
- [License](#-license)

---

## 🎯 Problem Statement

Managing personal finances is challenging in today's complex economic landscape:

- **📊 Data Overload**: People struggle to make sense of their financial data across multiple accounts and transactions
- **🤔 Poor Decision Making**: Lack of personalized insights leads to suboptimal spending and saving decisions
- **📉 No Predictive Analysis**: Traditional tools don't leverage AI to forecast future financial trends
- **⏰ Time Consuming**: Manual tracking and categorization of expenses takes significant time
- **🔒 Security Concerns**: Many finance apps lack robust security measures to protect sensitive financial data
- **💡 Limited Intelligence**: Existing solutions provide static reports without actionable, AI-driven recommendations

---

## ✨ Solution

**AI Finance** is an intelligent personal finance management platform that leverages cutting-edge AI technology to transform how you manage money:

🤖 **AI-Powered Insights** - Get personalized financial advice powered by Google's Gemini AI  
📊 **Smart Analytics** - Visualize your spending patterns with interactive dashboards  
🔐 **Bank-Level Security** - Protected by Arcjet security layer and Clerk authentication  
📧 **Smart Notifications** - Receive timely alerts about your financial health via Resend  
💳 **Transaction Tracking** - Automatically categorize and analyze your transactions  
📈 **Predictive Forecasting** - AI-driven predictions for future spending and savings

---

## 🎨 Features

### Core Functionality
- ✅ **User Authentication & Onboarding** - Secure sign-up/sign-in with Clerk
- ✅ **AI Financial Assistant** - Chat with Gemini AI for personalized advice
- ✅ **Transaction Management** - Add, edit, and categorize transactions
- ✅ **Budget Planning** - Set and track budgets with AI recommendations
- ✅ **Expense Analytics** - Visual insights into spending patterns
- ✅ **Income Tracking** - Monitor multiple income sources
- ✅ **Goal Setting** - Set financial goals with AI-powered milestones
- ✅ **Email Notifications** - Stay informed about your finances
- ✅ **Security Protection** - Rate limiting and DDoS protection

---

## 🛠 Tech Stack

### Frontend
- **[Next.js 15](https://nextjs.org/)** - React framework with App Router
- **[TypeScript](https://www.typescriptlang.org/)** - Type-safe development
- **[Tailwind CSS](https://tailwindcss.com/)** - Utility-first CSS framework
- **[shadcn/ui](https://ui.shadcn.com/)** - Beautiful UI components
- **[Recharts](https://recharts.org/)** - Data visualization library

### Backend
- **[Next.js API Routes](https://nextjs.org/docs/api-routes/introduction)** - Serverless API endpoints
- **[PostgreSQL](https://www.postgresql.org/)** - Relational database
- **[Prisma](https://www.prisma.io/)** - Next-generation ORM
- **[Neon](https://neon.tech/)** - Serverless Postgres hosting

### AI & Machine Learning
- **[Google Gemini AI](https://deepmind.google/technologies/gemini/)** - Advanced language model for financial insights
- **Natural Language Processing** - Understanding user queries and providing contextual advice

### Authentication & Security
- **[Clerk](https://clerk.com/)** - Complete user authentication
- **[Arcjet](https://arcjet.com/)** - Security and rate limiting

### Communication
- **[Resend](https://resend.com/)** - Modern email API for transactional emails

---

## 🔧 Tools Used

### Development
- **[Visual Studio Code](https://code.visualstudio.com/)** - Primary IDE
- **[Git](https://git-scm.com/)** - Version control
- **[GitHub](https://github.com/)** - Code repository and collaboration
- **[pnpm](https://pnpm.io/)** / **[npm](https://www.npmjs.com/)** - Package management

### Database Management
- **[Prisma Studio](https://www.prisma.io/studio)** - Database GUI
- **[Neon Console](https://neon.tech/)** - Database hosting and management

### API Testing & Development
- **[Postman](https://www.postman.com/)** - API testing and documentation
- **Browser DevTools** - Frontend debugging

### Deployment & Hosting
- **[Vercel](https://vercel.com/)** - Seamless Next.js deployment
- **[Neon](https://neon.tech/)** - Serverless PostgreSQL

### Monitoring & Analytics
- **[Vercel Analytics](https://vercel.com/analytics)** - Performance monitoring
- **[Sentry](https://sentry.io/)** *(Optional)* - Error tracking

---

## 🚀 Getting Started

### Prerequisites

- Node.js 18+ and npm/pnpm
- PostgreSQL database (Neon recommended)
- Clerk account
- Google Gemini API key
- Resend API key
- Arcjet API key

### Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/armaan-arora/aifinance.git
   cd aifinance
   ```

2. **Install dependencies**
   ```bash
   npm install
   # or
   pnpm install
   ```

3. **Set up environment variables**
   ```bash
   cp .env.example .env
   ```
   Fill in your API keys (see [Environment Variables](#-environment-variables))

4. **Set up the database**
   ```bash
   npx prisma generate
   npx prisma db push
   ```

5. **Run the development server**
   ```bash
   npm run dev
   # or
   pnpm dev
   ```

6. **Open your browser**
   Navigate to [http://localhost:3000](http://localhost:3000)

---

## 🔐 Environment Variables

Create a `.env` file in the root directory with the following variables:

```env
# Database
DATABASE_URL="postgresql://..."
DIRECT_URL="postgresql://..."

# Clerk Authentication
NEXT_PUBLIC_CLERK_PUBLISHABLE_KEY="pk_..."
CLERK_SECRET_KEY="sk_..."
NEXT_PUBLIC_CLERK_SIGN_IN_URL="/sign-in"
NEXT_PUBLIC_CLERK_SIGN_UP_URL="/sign-up"
NEXT_PUBLIC_CLERK_AFTER_SIGN_IN_URL="/onboarding"
NEXT_PUBLIC_CLERK_AFTER_SIGN_UP_URL="/onboarding"

# Google Gemini AI
GEMINI_API_KEY="..."

# Resend Email
RESEND_API_KEY="re_..."

# Arcjet Security
ARCJET_KEY="ajkey_..."
```

### Getting API Keys

- **Neon Database**: [neon.tech](https://neon.tech/)
- **Clerk**: [clerk.com](https://clerk.com/)
- **Gemini AI**: [ai.google.dev](https://ai.google.dev/)
- **Resend**: [resend.com](https://resend.com/)
- **Arcjet**: [arcjet.com](https://arcjet.com/)

---

## 🔮 Future Scope

### Planned Features

#### 🎯 Short-term (Next 3-6 months)
- [ ] **Bank Integration** - Connect real bank accounts via Plaid/Finicity
- [ ] **Bill Reminders** - Smart notifications for upcoming bills
- [ ] **Receipt Scanning** - OCR technology to digitize receipts
- [ ] **Multi-currency Support** - Track finances in multiple currencies
- [ ] **Dark Mode** - Eye-friendly dark theme
- [ ] **Mobile App** - React Native mobile application
- [ ] **Export Reports** - PDF/Excel financial reports

#### 🚀 Mid-term (6-12 months)
- [ ] **Investment Tracking** - Portfolio management and analysis
- [ ] **Tax Optimization** - AI-powered tax-saving suggestions
- [ ] **Family Accounts** - Shared financial management
- [ ] **Subscription Tracker** - Monitor and optimize recurring subscriptions
- [ ] **Debt Payoff Planner** - Strategic debt elimination strategies
- [ ] **Credit Score Monitoring** - Track and improve credit health
- [ ] **Voice Commands** - Alexa/Google Assistant integration

#### 🌟 Long-term (1+ years)
- [ ] **Robo-Advisor** - Automated investment recommendations
- [ ] **Financial Planning** - Long-term wealth building strategies
- [ ] **Marketplace** - Connect with financial advisors and services
- [ ] **Social Features** - Compare (anonymously) with peers
- [ ] **Blockchain Integration** - Crypto portfolio tracking
- [ ] **AI Spending Coach** - Proactive financial habit improvement
- [ ] **Open Banking API** - Platform for third-party integrations

### Technical Improvements
- [ ] Enhanced AI model fine-tuning for better predictions
- [ ] Real-time collaboration features
- [ ] Advanced caching strategies
- [ ] Micro-frontend architecture
- [ ] GraphQL API layer
- [ ] Comprehensive unit and E2E testing
- [ ] PWA (Progressive Web App) capabilities

---

## 🤝 Contributing

Contributions are what make the open-source community amazing! Any contributions you make are **greatly appreciated**.

1. Fork the Project
2. Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
3. Commit your Changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the Branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

---

## 📄 License

Distributed under the MIT License. See `LICENSE` file for more information.

---

## 👨‍💻 Author

**Armaan Arora**

- GitHub: [@armaan-arora](https://github.com/armaan-arora)
- LinkedIn: [Connect with me](https://linkedin.com/in/armaan-arora)

---

## 🙏 Acknowledgments

- [Next.js Documentation](https://nextjs.org/docs)
- [Clerk Documentation](https://clerk.com/docs)
- [Google Gemini AI](https://ai.google.dev/)
- [shadcn/ui](https://ui.shadcn.com/)
- [Vercel](https://vercel.com/)

---

<div align="center">
  <sub>Built with ❤️ by Armaan Arora</sub>
</div>

---

## 📞 Support

If you have any questions or need help, feel free to:

- 🐛 [Open an Issue](https://github.com/armaan-arora/aifinance/issues)
- 💬 [Start a Discussion](https://github.com/armaan-arora/aifinance/discussions)
- ⭐ Star this repository if you find it helpful!

---

**Made with Next.js, TypeScript, and AI** 🚀
