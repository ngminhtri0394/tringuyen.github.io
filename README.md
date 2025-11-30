# Tri Nguyen - Personal Homepage

A Jekyll-powered personal homepage for showcasing research, publications, blog posts, talks, grants, and awards.

## 🚀 Quick Start

### Prerequisites
- Ruby (version 2.7 or higher)
- Bundler gem

### Local Development

1. **Install dependencies:**
   ```bash
   bundle install
   ```

2. **Run the development server:**
   ```bash
   bundle exec jekyll serve
   ```

3. **View your site at:** `http://localhost:4000`

## 📁 Project Structure

```
.
├── _config.yml          # Site configuration
├── _data/               # Data files (easy to edit!)
│   ├── publications.yml # Your publications list
│   ├── talks.yml        # Talks and presentations
│   ├── grants.yml       # Grants and funding
│   ├── awards.yml       # Awards and recognition
│   └── cv.yml           # CV information
├── _includes/           # Reusable HTML components
├── _layouts/            # Page templates
├── _posts/              # Blog posts (Markdown)
├── assets/
│   ├── css/             # Stylesheets
│   └── js/              # JavaScript files
├── index.md             # Homepage
└── Gemfile              # Ruby dependencies
```

## ✍️ Adding Content

### Adding a New Blog Post

1. Create a new file in `_posts/` with the format: `YYYY-MM-DD-title.md`
2. Add front matter at the top:
   ```yaml
   ---
   layout: post
   title: "Your Post Title"
   date: 2024-12-01
   tags: [Tag1, Tag2]
   read_time: 5
   excerpt: "Brief description of your post"
   ---
   ```
3. Write your content in Markdown below the front matter.

### Adding a Publication

Edit `_data/publications.yml` and add:
```yaml
- title: "Your Paper Title"
  authors: "Author 1, Author 2, Author 3"
  venue: "Journal or Conference Name"
  year: 2025
  description: "Brief description"
  doi: "https://doi.org/..."
```

### Adding a Talk

Edit `_data/talks.yml` and add:
```yaml
- title: "Talk Title"
  venue: "Conference Name"
  year: 2025
  description: "Brief description"
  slides: "link-to-slides"  # optional
  video: "link-to-video"    # optional
```

### Adding a Grant

Edit `_data/grants.yml` and add:
```yaml
- title: "Grant Title"
  amount: "$50,000"
  agency: "Funding Agency"
  period: "2024-2025"
  description: "Brief description"
```

### Adding an Award

Edit `_data/awards.yml` and add:
```yaml
- title: "Award Title"
  organization: "Organization Name"
  year: 2024
  icon: "fa-trophy"  # Options: fa-trophy, fa-medal, fa-star, fa-award
  description: "Brief description"
```

### Updating CV

Edit `_data/cv.yml` to modify education entries or the PDF download link.

## ⚙️ Configuration

Edit `_config.yml` to update:
- Site title and description
- Author information (name, email, social links)
- Base URL settings

## 🎨 Customization

- **Styles:** Edit `assets/css/style.css`
- **Scripts:** Edit `assets/js/script.js`
- **Layouts:** Modify files in `_layouts/`
- **Components:** Modify files in `_includes/`

## 🌐 Deployment

This site is configured for GitHub Pages. Simply push to the `main` branch and GitHub will automatically build and deploy your site.

## 📝 License

© Tri Nguyen. All rights reserved.