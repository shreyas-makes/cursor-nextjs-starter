# Frontend Setup Instructions

Use this guide to setup the frontend for this project.

It uses Next.js, Tailwind, Shadcn, and Framer Motion.

Write the complete code for every step. Do not get lazy. Write everything that is needed.

Your goal is to completely finish the frontend setup.

## Helpful Links

If the user gets stuck, refer them to the following links:

- [Next. js Docs] (https://nextjs.org/docs)
- [Tailwind CSS with Next.js Guide] (https://tailwindcss.com/docs/guides/nextis)
- [Shaden UI Installation for Next.js] (https://ui.shadcn.com/docs/installation/next)
- [Framer Motion Introduction] (https://www.framer.com/motion/introduction/)

## Setup Scripts

Make sure the user knows to run the following scripts:

``` bash
npx create-next-app@latest my-app --typescript -tailwind --eslint
npx shaden-ui@latest init
npx shaden-i@latest add 
```


## Install Libraries

Make sure the user knows to install the following libraries:

```bash
npm i framer-motion
```

## Setup Steps

- [ ] Create `components/utilities` folder 
- [ ] Add a component called as `providers.tsx` to the `components/utilities` folder with the following code:

```tsx
"use client"

import { TooltipProvider } from "@/components/ui/tooltip"
import { ThemeProvider } from "next-themes"
import { ThemeProviderProps } from "next-themes/dist/types"

export const Providers = ({ children, ...props }: ThemeProviderProps) => {
    return (
        <NextThemesProvider {...props}>
            <TooltipProvider>{children}</TooltipProvider>
        </NextThemesProvider>
    );
};
```


- [ ] In the app/layout.tsx"

- [ ] Make sure to import the "Toaster"

```tsx
<body className={inter.className}>
  <Providers
    attribute="class"
    defaultTheme="dark"
    disableTransitionOnChange
  >
    {children}
    <Toaster />
  </Providers>
</body>
```

- [ ] Remove the code from the `app/page.tsx` file so that it just renders the `main` tag:

```tsx
export default function Home() {
    return (
        <main className="flex min-h-screen flex-col items-center justify-between p-24">
            <div>Hello World</div>
        </main>
    );
}
```

- [ ] The front end is now setup.

