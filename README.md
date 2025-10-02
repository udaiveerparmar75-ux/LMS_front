# RMT ENGINEERING - Lead Management System

A modern, responsive lead management system built with Next.js, TypeScript, and Tailwind CSS.

## Features

- **Modern Authentication UI**: Beautiful login and registration pages with glass morphism effects
- **Form Validation**: Comprehensive client-side validation using Zod and React Hook Form
- **Responsive Design**: Mobile-first design that works on all devices
- **TypeScript**: Full type safety throughout the application
- **Tailwind CSS**: Utility-first CSS framework for rapid UI development

## Tech Stack

- **Framework**: Next.js 14 with App Router
- **Language**: TypeScript
- **Styling**: Tailwind CSS
- **Form Handling**: React Hook Form
- **Validation**: Zod
- **Icons**: Lucide React

## Getting Started

### Prerequisites

- Node.js 18+ 
- npm or yarn

### Installation

1. Clone the repository:
   ```bash
   git clone <repository-url>
   cd LMS\ front
   ```

2. Install dependencies:
   ```bash
   npm install
   ```

3. Run the development server:
   ```bash
   npm run dev
   ```

4. Open [http://localhost:3000](http://localhost:3000) in your browser

## Project Structure

```
├── app/
│   ├── globals.css          # Global styles and Tailwind imports
│   ├── layout.tsx           # Root layout component
│   ├── page.tsx             # Home page (redirects to login)
│   ├── login/
│   │   └── page.tsx         # Login page
│   └── register/
│       └── page.tsx         # Registration page
├── package.json             # Dependencies and scripts
├── tailwind.config.js       # Tailwind CSS configuration
├── tsconfig.json           # TypeScript configuration
└── README.md               # This file
```

## Pages

### Login Page (`/login`)
- Username/password authentication
- Form validation
- Password visibility toggle
- Remember me option
- Forgot password link
- Link to registration page

### Registration Page (`/register`)
- Complete user registration form
- Fields: First name, Last name, Username, Email, Phone, Company, Password
- Password confirmation validation
- Terms and conditions checkbox
- Link to login page

## Form Validation

Both forms include comprehensive validation:
- Required field validation
- Email format validation
- Password strength requirements
- Password confirmation matching
- Real-time error display

## Styling

The application uses a modern design with:
- Gradient backgrounds
- Glass morphism effects
- Smooth transitions and animations
- Consistent color scheme
- Mobile-responsive layout

## Customization

### Colors
The primary color scheme can be customized in `tailwind.config.js`:
```javascript
colors: {
  primary: {
    // Customize these values
    500: '#3b82f6',
    600: '#2563eb',
    700: '#1d4ed8',
  }
}
```

### Company Branding
Update the company name and branding in:
- Page titles in `app/layout.tsx`
- Company name in login and registration pages
- Logo/icon components

## Development

### Available Scripts

- `npm run dev` - Start development server
- `npm run build` - Build for production
- `npm run start` - Start production server
- `npm run lint` - Run ESLint

### Adding New Features

1. Create new pages in the `app/` directory
2. Add form validation schemas using Zod
3. Implement API routes in `app/api/` (when needed)
4. Update navigation and routing as needed

## Production Deployment

1. Build the application:
   ```bash
   npm run build
   ```

2. Deploy to your preferred platform (Vercel, Netlify, etc.)

## Contributing

1. Fork the repository
2. Create a feature branch
3. Make your changes
4. Test thoroughly
5. Submit a pull request

## License

This project is licensed under the MIT License.
