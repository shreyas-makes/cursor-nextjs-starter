# Next.js Prompt Starter Kit for Cursor AI

This starter kit provides a foundation for creating Next.js projects using Cursor AI. Follow these steps to get started:

## Setup

1. Initialize a new Next.js project:
   ```
   npx create-next-app@latest my-project
   cd my-project
   ```

2. Install additional dependencies:
   ```
   npm install @radix-ui/react-icons class-variance-authority clsx tailwind-merge nuqs
   ```

3. Set up Tailwind CSS and Shadcn UI:
   ```
   npx shadcn-ui@latest init
   ```

## Development Workflow

1. Create new components in the `/components` directory:
   ```
   npx shadcn-ui@latest add button
   ```

2. Implement server components in `/app` directory.

3. Use Cursor AI for code generation and refactoring:
   - Describe the desired functionality
   - Specify component names and file paths
   - Request TypeScript interfaces when needed

4. Optimize performance:
   - Minimize client-side components
   - Implement code-splitting and lazy loading
   - Use Next.js Image component for optimized images

5. Style components using Tailwind CSS:
   - Utilize utility classes
   - Create responsive designs with mobile-first approach

6. Implement routing and data fetching using Next.js App Router.

7. Manage URL state with `nuqs` when necessary.

8. Utilize the `@/prompts` folder:
   - Set up frontend prompts for UI components and layouts
   - Create backend prompts for API routes and server-side logic
   - Use prompts to generate consistent code across the project

## Best Practices

- Follow TypeScript best practices
- Use functional components and hooks
- Implement error boundaries and fallback UI
- Optimize for Core Web Vitals

## Deployment

Deploy your Next.js application using Vercel or your preferred hosting platform.

Remember to customize this starter kit based on your project's specific requirements and team preferences.

## Using @/prompts Folder

The `@/prompts` folder is a powerful tool for setting up both frontend and backend components of your Next.js application:

### Frontend Prompts
1. Create prompts for common UI components (e.g., forms, modals, cards)
2. Define layout structures and responsive designs
3. Generate consistent styling using Tailwind CSS classes

### Backend Prompts
1. Set up API route templates
2. Create database models and query structures
3. Define authentication and authorization logic

By utilizing the `@/prompts` folder, you can ensure consistency across your project and speed up development by generating boilerplate code for both frontend and backend components.