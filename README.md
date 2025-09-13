# Yichen Peng's Personal Website

This is my personal website built with Jekyll and hosted on GitHub Pages. The site is based on a fork of **Jekyll Now** from [this repository](https://github.com/barryclark/jekyll-now) and uses a design inspired by [Jon Barron's website](https://jonbarron.info/).

## About
This website showcases my research work, professional projects, and other activities. It's organized into three main sections:
- **Research**: Academic publications and research projects
- **Professional Projects**: Industry work and professional experience  
- **Other Projects**: Side projects, coursework, and personal work

## Customization Guide
To customize this website for your own use:

1. **Update Personal Information**:
   - Edit `_config.yml` to update your name, email, GitHub username, and other social links
   - Replace the profile photo in `images/circle_bw_crop.jpg` with your own photo
   - Update the bio and contact links in `_layouts/default.html`

2. **Add Your Content**:
   - Create new posts in the `_posts/` folder using the example format
   - Use categories: `research`, `Intel` (or your company name), or other categories for different sections
   - Add your project images to the `images/` folder and thumbnails to `tn/images/`

3. **Customize Sections**:
   - Edit section headers in `_layouts/default.html` (e.g., change "Professional Projects" to match your industry)
   - Update the research interests and other descriptive text 



## issues
* In general, jekyll will try to build a full page for every post. I skip that by forcing `permalink: /`. This creates multiple entries in sitemap.xml for index.html but is otherwise fine. 
* If you want multiple paragraphs, consider using `excerpt_separator: <!--more-->` in `_config.yml`, for my own use I didn't need this. 
* My own posts have lots of extra stuff left over from my old jekyll design ("author", long descriptions, etc.), feel free to ignore them
* I use thumbnails, so I can upload arbitrary sized images but then only display small ones. The `_make_thumbnails.sh` script generates them and the html template looks in `tn/` for all images. 
* I have three categories of post with slightly differerent formatting, so changing sizing requires edits in multiple paces. 
