# Happy Hacking Space - Website Code

![image](https://github.com/user-attachments/assets/9ca41245-8137-4f4b-ac2c-4a55ac22159b)

Welcome to the website for Happy Hacking Space, a community-driven platform that brings together technology enthusiasts, creators, and innovators.

## About Happy Hacking Space

Happy Hacking Space is a community-driven, collaborative environment where individuals with shared interests in technology, science, and creative endeavors come together to experiment, learn, and innovate through playful exploration and clever problem-solving. We embrace the hacker spirit of curiosity and creativity, operating as a space for collaboration and skill-sharing while fostering a sense of fun in pushing the boundaries of what is possible.

## What is Hacking?

In our community, hacking represents the spirit of playful intelligence and exploration. As RMS puts it in "On Hacking":

> Defining hacking can be challenging due to its variable nature. However, a common trait among many hackers is their playful, intelligent, and exploratory mindset. Thus, hacking means exploring the boundaries of what is possible with a playful spirit. Activities that demonstrate playful intelligence have hack value.

## Adding a New Article to the App

**Hello, friend!**

I'm writing my first blog post to explain how you can publish your own article on the HHS blog system.

### How the HHS Blog System Works

Before you start, here’s how the HHS blog system operates:

- The HHS blog system requires blog articles to be in **MDX file format** (Markdown + JSX).
- The application fetches MDX files from the `content/blog/` directory to render blog posts on the website.
- If your article includes images, they should be stored in the `/public/blog/` folder.
    - Create a **new folder named after the publishing date** to organize images properly.
    - Example structure for an article published on **February 26, 2025**:
        - `/public/blog/26022025/image1.jpg`
        - `/public/blog/26022025/image2.jpg`
        - `/public/blog/26022025/image3.jpg`

### Writing Your MDX Blog Post

Once your image assets are ready, it's time to create the MDX file.

Your blog post must start with the following **frontmatter**:
```
---
title: "Your Post Title"                 # The title of your article
subtitle: "Your Post Subtitle"           # (Optional) A brief subtitle
summary: "A brief summary of your post"  # Short summary for previews
publishedAt: "YYYY-MM-DD"                # The publication date
author: "Author Name"                    # Your name (the author)
tags: ["tag1", "tag2"]                   # Relevant keywords for your post
---

```

### Explanation of the Frontmatter Fields

- **`title`** – The main title of your article.
- **`subtitle`** – An optional subtitle.
- **`summary`** – A short description of your article for previews.
- **`publishedAt`** – The date when you are publishing the post on HHS (format: `YYYY-MM-DD`).
- **`author`** – Your name, indicating who wrote the article.
- **`tags`** – At least **1-2 relevant keywords** in an array format, e.g., `["technology", "web-development"]`.

### Writing the Markdown Content

After the frontmatter, you can write the main content of your article using Markdown syntax.
```
## Your Post Title

Write the content of your post here. You can use Markdown for formatting.

### Example Code Block  

To include code snippets, use fenced code blocks:

```javascript
console.log("This is a test post");

const test = async () => {
    await new Promise((resolve) => setTimeout(resolve, 1000));
    console.log("This is a test post");
};

test();

```

### Adding Images

To include images in your article, use the following format:
```
<img src="/blog/26022025/image1.jpg" alt="A description of your image" style={{ width: "50%" }} />
```

### Publishing Your Blog Post
Follow these steps to submit your blog post:

1. **Fork the `landing-frontend-app` repository**.
2. **Push your commits**, including the new blog post and any image assets.
3. Once you’re sure everything is correct, **create a pull request**.
4. Wait for a reviewer to approve your changes before your article is published.

That’s it! You're now ready to publish your first article on the HHS blog. 🎉

Example blog post:
```
---
title: "Your Post Title"                 # The title of your article
subtitle: "Your Post Subtitle"           # (Optional) A brief subtitle
summary: "A brief summary of your post"  # Short summary for previews
publishedAt: "YYYY-MM-DD"                # The publication date
author: "Author Name"                    # Your name (the author)
tags: ["tag1", "tag2"]                   # Relevant keywords for your post
---

## Your Post Title

Write the content of your post here. You can use Markdown for formatting.

### Example Code Block  

To include code snippets, use fenced code blocks:

```javascript
console.log("This is a test post");

const test = async () => {
    await new Promise((resolve) => setTimeout(resolve, 1000));
    console.log("This is a test post");
};

test();

<img src="/blog/26022025/image1.jpg" alt="A description of your image" style={{ width: "50%" }} />


```


## Technical Stack

This is a modern web application built with:

- [Next.js](https://nextjs.org) - React framework for production
- MDX for content management
- Tailwind CSS for styling
- TypeScript for type safety

## Getting Started

1. Clone the repository
2. Install dependencies:

   ```bash
   npm install
   # or
   yarn install
   # or
   pnpm install
   # or
   bun install
   ```

3. Run the development server:

   ```bash
   npm run dev
   # or
   yarn dev
   # or
   pnpm dev
   # or
   bun dev
   ```

4. Open [http://localhost:3000](http://localhost:3000) in your browser

## Community

Join our community of hackers, makers, and technology enthusiasts. Together, we explore the boundaries of what's possible through collaborative learning and creative problem-solving.
