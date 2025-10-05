# Personal website

This is the source code for the personal portfolio page of Chris Vos

## Local Development

### Prerequisites
- Ruby (with bundler)

### Setup
1. Install dependencies:
   ```bash
   bundle install --path vendor/bundle
   ```

2. Build the site:
   ```bash
   bundle exec jekyll build
   ```

3. Serve locally:
   ```bash
   bundle exec jekyll serve
   ```

The site will be available at `http://localhost:4000`

### File Structure
- `_config.yml` - Jekyll configuration
- `_includes/` - Reusable HTML components
- `_layouts/` - Page templates
- `_sass/` - Sass stylesheets
- `discography/` - Discography posts and pages
- `live/` - Live performance posts and pages