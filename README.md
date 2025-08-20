@import "tailwindcss";
@import "tw-animate-css";

@custom-variant dark (&:is(.dark *));

:root {
  --background: oklch(1 0 0); /* Pure white background */
  --foreground: oklch(0.145 0 0); /* Black text */
  --card: oklch(0.98 0 0); /* Light grey card background */
  --card-foreground: oklch(0.145 0 0); /* Black card text */
  --popover: oklch(1 0 0); /* White popover */
  --popover-foreground: oklch(0.145 0 0); /* Black popover text */
  --primary: oklch(0.55 0.15 142); /* Environmental green #00b140 */
  --primary-foreground: oklch(1 0 0); /* White text on green */
  --secondary: oklch(0.96 0 0); /* Light grey secondary */
  --secondary-foreground: oklch(0.145 0 0); /* Black secondary text */
  --muted: oklch(0.96 0 0); /* Muted grey background */
  --muted-foreground: oklch(0.45 0 0); /* Muted grey text */
  --accent: oklch(0.55 0.15 142); /* Green accent matching primary */
  --accent-foreground: oklch(1 0 0); /* White accent text */
  --destructive: oklch(0.577 0.245 27.325); /* Red for destructive actions */
  --destructive-foreground: oklch(1 0 0); /* White destructive text */
  --border: oklch(0.9 0 0); /* Light border */
  --input: oklch(1 0 0); /* White input background */
  --ring: oklch(0.55 0.15 142 / 0.5); /* Green focus ring */
  --chart-1: oklch(0.55 0.15 142); /* Green chart color */
  --chart-2: oklch(0.7 0.15 85); /* Yellow-green chart color */
  --chart-3: oklch(0.4 0.12 160); /* Dark green chart color */
  --chart-4: oklch(0.6 0.18 120); /* Light green chart color */
  --chart-5: oklch(0.35 0.1 140); /* Forest green chart color */
  --radius: 0.625rem;
  --sidebar: oklch(0.98 0 0); /* Light sidebar */
  --sidebar-foreground: oklch(0.145 0 0); /* Black sidebar text */
  --sidebar-primary: oklch(0.55 0.15 142); /* Green sidebar primary */
  --sidebar-primary-foreground: oklch(1 0 0); /* White sidebar primary text */
  --sidebar-accent: oklch(0.96 0 0); /* Light sidebar accent */
  --sidebar-accent-foreground: oklch(0.145 0 0); /* Black sidebar accent text */
  --sidebar-border: oklch(0.9 0 0); /* Light sidebar border */
  --sidebar-ring: oklch(0.55 0.15 142 / 0.5); /* Green sidebar ring */
}

.dark {
  --background: oklch(0.145 0 0); /* Dark background */
  --foreground: oklch(0.985 0 0); /* Light text */
  --card: oklch(0.2 0 0); /* Dark card */
  --card-foreground: oklch(0.985 0 0); /* Light card text */
  --popover: oklch(0.145 0 0); /* Dark popover */
  --popover-foreground: oklch(0.985 0 0); /* Light popover text */
  --primary: oklch(0.6 0.15 142); /* Brighter green for dark mode */
  --primary-foreground: oklch(0.145 0 0); /* Dark text on green */
  --secondary: oklch(0.25 0 0); /* Dark secondary */
  --secondary-foreground: oklch(0.985 0 0); /* Light secondary text */
  --muted: oklch(0.25 0 0); /* Dark muted */
  --muted-foreground: oklch(0.7 0 0); /* Light muted text */
  --accent: oklch(0.6 0.15 142); /* Bright green accent */
  --accent-foreground: oklch(0.145 0 0); /* Dark accent text */
  --destructive: oklch(0.6 0.25 25); /* Bright red destructive */
  --destructive-foreground: oklch(0.985 0 0); /* Light destructive text */
  --border: oklch(0.25 0 0); /* Dark border */
  --input: oklch(0.25 0 0); /* Dark input */
  --ring: oklch(0.6 0.15 142 / 0.5); /* Green focus ring */
  --chart-1: oklch(0.6 0.15 142); /* Bright green chart */
  --chart-2: oklch(0.75 0.15 85); /* Bright yellow-green chart */
  --chart-3: oklch(0.45 0.12 160); /* Medium green chart */
  --chart-4: oklch(0.65 0.18 120); /* Bright light green chart */
  --chart-5: oklch(0.4 0.1 140); /* Dark forest green chart */
  --sidebar: oklch(0.2 0 0); /* Dark sidebar */
  --sidebar-foreground: oklch(0.985 0 0); /* Light sidebar text */
  --sidebar-primary: oklch(0.6 0.15 142); /* Bright green sidebar primary */
  --sidebar-primary-foreground: oklch(0.145 0 0); /* Dark sidebar primary text */
  --sidebar-accent: oklch(0.25 0 0); /* Dark sidebar accent */
  --sidebar-accent-foreground: oklch(0.985 0 0); /* Light sidebar accent text */
  --sidebar-border: oklch(0.25 0 0); /* Dark sidebar border */
  --sidebar-ring: oklch(0.6 0.15 142 / 0.5); /* Green sidebar ring */
}

@theme inline {
  --color-background: var(--background);
  --color-foreground: var(--foreground);
  --color-card: var(--card);
  --color-card-foreground: var(--card-foreground);
  --color-popover: var(--popover);
  --color-popover-foreground: var(--popover-foreground);
  --color-primary: var(--primary);
  --color-primary-foreground: var(--primary-foreground);
  --color-secondary: var(--secondary);
  --color-secondary-foreground: var(--secondary-foreground);
  --color-muted: var(--muted);
  --color-muted-foreground: var(--muted-foreground);
  --color-accent: var(--accent);
  --color-accent-foreground: var(--accent-foreground);
  --color-destructive: var(--destructive);
  --color-destructive-foreground: var(--destructive-foreground);
  --color-border: var(--border);
  --color-input: var(--input);
  --color-ring: var(--ring);
  --color-chart-1: var(--chart-1);
  --color-chart-2: var(--chart-2);
  --color-chart-3: var(--chart-3);
  --color-chart-4: var(--chart-4);
  --color-chart-5: var(--chart-5);
  --radius-sm: calc(var(--radius) - 4px);
  --radius-md: calc(var(--radius) - 2px);
  --radius-lg: var(--radius);
  --radius-xl: calc(var(--radius) + 4px);
  --color-sidebar: var(--sidebar);
  --color-sidebar-foreground: var(--sidebar-foreground);
  --color-sidebar-primary: var(--sidebar-primary);
  --color-sidebar-primary-foreground: var(--sidebar-primary-foreground);
  --color-sidebar-accent: var(--sidebar-accent);
  --color-sidebar-accent-foreground: var(--sidebar-accent-foreground);
  --color-sidebar-border: var(--sidebar-border);
  --color-sidebar-ring: var(--sidebar-ring);
}

@layer base {
  * {
    @apply border-border outline-ring/50;
  }
  body {
    @apply bg-background text-foreground;
  }
}
