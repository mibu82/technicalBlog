# technicalBlog

잡다한 콘텐츠를 다루는 블로그입니다. 주로 기술 트렌드, 기술 관련 산업 동향 등을 다룹니다.

## GitHub Pages Setup

This repository is configured to use GitHub Pages as a documentation storage platform. The site is built automatically using Jekyll and GitHub Actions.

### 🌐 Live Site

The blog will be available at: `https://mibu82.github.io/technicalBlog/`

### 📝 Adding New Content

To add new blog posts or documentation:

1. Create a new file in the `_posts` directory
2. Name it using the format: `YYYY-MM-DD-title.md`
3. Add front matter at the top:
   ```yaml
   ---
   layout: post
   title: "Your Post Title"
   date: YYYY-MM-DD HH:MM:SS +0900
   categories: [category1, category2]
   tags: [tag1, tag2]
   ---
   ```
4. Write your content in Markdown
5. Commit and push to the main branch

### 🛠️ Local Development

To run the site locally:

```bash
# Install dependencies
bundle install

# Run Jekyll server
bundle exec jekyll serve

# Visit http://localhost:4000/technicalBlog/
```

### 🚀 Deployment

The site automatically deploys via GitHub Actions when changes are pushed to the main branch. The workflow is defined in `.github/workflows/pages.yml`.

### 📁 Repository Structure

```
technicalBlog/
├── _posts/           # Blog posts (YYYY-MM-DD-title.md format)
├── _config.yml       # Jekyll configuration
├── index.md          # Home page
├── Gemfile           # Ruby dependencies
├── .github/
│   └── workflows/
│       └── pages.yml # GitHub Actions deployment workflow
└── README.md         # This file
```

### ⚙️ Configuration

The site configuration is in `_config.yml`. You can customize:
- Site title and description
- URL and baseurl
- Theme and plugins
- Collections and permalinks

### 🎨 Theme

The site uses the [Minima](https://github.com/jekyll/minima) theme by default. You can customize it or switch to another Jekyll theme.
