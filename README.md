# My GitHub Pages Blog

This is a personal blog created with Jekyll and the Chirpy theme, hosted on GitHub Pages.

## Getting Started

### Local Development

1. Clone this repository:
   ```bash
   git clone https://github.com/yourusername/yourusername.github.io.git
   cd yourusername.github.io
   ```

2. Install Server and dependencies:
   ```bash
   # For macOS
   docker build -t jekyll-blog .
   docker run --rm -p 4000:4000 -v $(pwd):/site jekyll-blog bundle exec jekyll serve --host 0.0.0.0 --livereload
   ```

3. Open your browser and navigate to `http://localhost:4000`

### Adding New Posts

1. Create a new Markdown file in the `_posts` directory with the naming convention: `YYYY-MM-DD-title.md`
2. Add the front matter at the top of the file:
   ```yaml
   ---
   title: "Your Post Title"
   date: YYYY-MM-DD HH:MM:SS -0000
   categories: [Category1, Category2]
   tags: [tag1, tag2]
   ---
   ```
3. Write your post content in Markdown below the front matter

## Customization

- Edit `_config.yml` to update site settings
- Add your avatar image to `assets/img/avatar.jpg`
- Customize the theme by modifying files in `_sass`

## Deployment

The site is automatically deployed when changes are pushed to the main branch.

## License

This project is licensed under the MIT License - see the LICENSE file for details.

## Reference

https://chirpy.cotes.page/