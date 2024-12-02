# Next.js E-commerce Store

A modern, full-featured e-commerce store built with Next.js 13, TypeScript, Tailwind CSS, and MongoDB.

## Features

- 🛍️ Product listing and details
- 🔐 User authentication (signup, login, logout)
- 📧 Email verification
- 🛒 Shopping cart functionality
- 💳 Secure user sessions
- 🎨 Modern UI with Tailwind CSS
- 📱 Fully responsive design
- 🔒 Protected routes
- 🗄️ MongoDB integration

## Tech Stack

- **Frontend:**
  - Next.js 13 (App Router)
  - TypeScript
  - Tailwind CSS
  - Shadcn UI Components
  - React Hook Form
  - Zod Validation

- **Backend:**
  - MongoDB
  - NextAuth.js
  - Node.js
  - Mongoose

- **Authentication:**
  - JWT
  - Bcrypt for password hashing

## Getting Started

### Prerequisites

- Node.js 16.8 or later
- MongoDB database
- npm or yarn

### Installation

1. Clone the repository:
   ```bash
   git clone <repository-url>
   cd nextjs-ecommerce
   ```

2. Install dependencies:
   ```bash
   npm install
   ```

3. Set up environment variables:
   Create a `.env` file in the root directory with the following variables:
   ```env
   MONGODB_URI=your_mongodb_connection_string
   NEXTAUTH_SECRET=your_nextauth_secret
   NEXTAUTH_URL=http://localhost:3000
   EMAIL_HOST=your_email_host
   EMAIL_PORT=your_email_port
   EMAIL_USER=your_email_username
   EMAIL_PASSWORD=your_email_password
   EMAIL_FROM=your_sender_email
   NEXT_PUBLIC_APP_URL=http://localhost:3000
   ```

4. Seed the database:
   ```bash
   node scripts/seed.js
   ```

5. Start the development server:
   ```bash
   npm run dev
   ```

6. Open [http://localhost:3000](http://localhost:3000) in your browser.

## Project Structure

```
├── app/                    # Next.js 13 app directory
│   ├── api/               # API routes
│   ├── (routes)/         # App routes
│   └── layout.tsx        # Root layout
├── components/            # React components
│   ├── ui/               # UI components
│   └── ...               # Other components
├── lib/                   # Utility functions
│   ├── auth/             # Authentication logic
│   ├── models/           # MongoDB models
│   └── services/         # Business logic
├── providers/            # React context providers
└── public/               # Static assets
```

## Features in Detail

### Authentication
- Secure user registration with email verification
- JWT-based authentication
- Protected routes with middleware
- Session management

### Products
- Product listing with pagination
- Product details
- Category filtering
- Stock management

### User Interface
- Responsive design
- Modern UI components
- Toast notifications
- Form validation
- Loading states

## Development

### Available Scripts

- `npm run dev` - Start development server
- `npm run build` - Build for production
- `npm start` - Start production server
- `npm run lint` - Run ESLint

### Database Seeding

The project includes  with initial products:



## Contributing

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add some amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Acknowledgments

- [Next.js](https://nextjs.org/)
- [Tailwind CSS](https://tailwindcss.com/)
- [MongoDB](https://www.mongodb.com/)
- [NextAuth.js](https://next-auth.js.org/)
- [Shadcn UI](https://ui.shadcn.com/)
