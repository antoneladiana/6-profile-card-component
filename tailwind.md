# Step-by-Step Guide: Setting Up Tailwind CSS v4 (CLI)

Follow these steps to set up Tailwind CSS v4 from scratch using the Tailwind CLI.

### Step 1: Initialize Your Project Folder

Open your terminal inside your project directory and initialize a new Node.js project:

```bash
npm init -y
```

### Step 2: Install Tailwind CSS & CLI

Install the latest Tailwind CSS v4 package and its command-line tool:

```bash
npm install tailwindcss @tailwindcss/cli
```

### Step 3: Create Your Input CSS File

Create a `src` folder and an input CSS file inside it:

```bash
mkdir src
touch src/input.css
```

Open `src/input.css` and add the Tailwind import directive:

```css
@import "tailwindcss";
```

### Step 4: Start the Build Process

Run the Tailwind CLI build process with the `--watch` flag:

```bash
npx @tailwindcss/cli -i ./src/input.css -o ./dist/output.css --watch
```

### Step 5: Link Output CSS in Your HTML

Create your HTML file (e.g., `src/index.html`) and link the generated `output.css` file inside the `<head>`:

```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Tailwind v4 Project</title>
    <link rel="stylesheet" href="./output.css" />
  </head>
  <body>
    <h1 class="text-3xl font-bold underline">Hello world!</h1>
  </body>
</html>
```
