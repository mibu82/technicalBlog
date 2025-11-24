# Contributing to Technical Blog

This guide explains how to add and manage content in this documentation repository.

## Adding Blog Posts

### 1. Create a New Post File

Create a new file in the `_posts` directory with the naming format:

```
_posts/YYYY-MM-DD-title-of-your-post.md
```

For example:
- `_posts/2025-11-24-getting-started-with-kubernetes.md`
- `_posts/2025-11-25-python-best-practices.md`

### 2. Add Front Matter

Every post must start with YAML front matter:

```yaml
---
layout: post
title: "Your Post Title"
date: 2025-11-24 14:30:00 +0900
categories: [technology, tutorial]
tags: [python, docker, kubernetes]
---
```

### 3. Write Content in Markdown

After the front matter, write your content using Markdown:

```markdown
# Main Heading

Your introduction paragraph...

## Subheading

- Bullet point 1
- Bullet point 2

### Code Examples

\`\`\`python
def hello_world():
    print("Hello, World!")
\`\`\`

## Conclusion

Wrap up your thoughts...
```

## Adding Documentation Pages

### Static Pages

Create `.md` files in the root directory or in a dedicated folder:

```
docs/
├── getting-started.md
├── api-reference.md
└── tutorials/
    ├── tutorial-1.md
    └── tutorial-2.md
```

Each page should have front matter:

```yaml
---
layout: page
title: "Getting Started"
permalink: /getting-started/
---
```

## Markdown Features

### Text Formatting

- **Bold**: `**bold text**`
- *Italic*: `*italic text*`
- `Code`: `` `code` ``

### Links

- Internal: `[Link Text](/path/to/page)`
- External: `[GitHub](https://github.com)`

### Images

```markdown
![Alt text](/assets/images/image.png)
```

Store images in an `assets/images/` directory.

### Tables

```markdown
| Column 1 | Column 2 | Column 3 |
|----------|----------|----------|
| Data 1   | Data 2   | Data 3   |
```

### Code Blocks

Use triple backticks with language specification:

````markdown
```javascript
function example() {
  console.log("Hello");
}
```
````

## Organizing Content

### Categories

Use categories to group related posts:

```yaml
categories: [tutorials, technology]
```

### Tags

Use tags for more specific topics:

```yaml
tags: [python, docker, ci-cd, devops]
```

## Local Preview

To preview your changes locally before committing:

1. Install Ruby and Bundler
2. Run:
   ```bash
   bundle install
   bundle exec jekyll serve
   ```
3. Visit `http://localhost:4000/technicalBlog/`

## Deployment

Changes are automatically deployed when merged to the main branch via GitHub Actions.

## Content Guidelines

### Writing Style

- Use clear, concise language
- Break content into sections with headings
- Include code examples where relevant
- Add images or diagrams for complex concepts

### File Naming

- Use lowercase letters
- Separate words with hyphens
- Use descriptive names
- Follow date format for posts: `YYYY-MM-DD-title.md`

### Commit Messages

Use clear commit messages:

- `Add post about Docker containers`
- `Update getting started guide`
- `Fix typo in Kubernetes tutorial`

## Questions?

If you have questions about contributing, please open an issue on GitHub.
