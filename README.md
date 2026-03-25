# G Web AI Drafts

Creates single or multiple draft posts via the WordPress REST API with Yoast SEO fields, featured images, categories, and tags using WordPress authentication. Ideal for bulk content creation workflows and automation.

## Table of Contents
- [Overview](#overview)
- [Features](#features)
- [Installation](#installation)
- [Usage](#usage)
- [Requirements](#requirements)
- [Configuration](#configuration)
- [Changelog](#changelog)
- [License](#license)
- [Contributing](#contributing)

---

## Overview
G Web AI Drafts allows WordPress site owners or developers to programmatically create draft posts in bulk. Each post can include:  
- Yoast SEO metadata  
- Featured images  
- Categories and tags  

The plugin authenticates using standard WordPress REST API credentials, making it suitable for multisite installations or remote content automation workflows.

---

## Features
- Create single or multiple draft posts via REST API  
- Automatically assign Yoast SEO fields (title, meta description, focus keywords)  
- Assign featured images programmatically  
- Map categories and tags automatically  
- Supports WordPress authentication for secure API usage  
- Optimized for bulk content creation and automated workflows  

---

## Installation
1. Download the plugin ZIP from [GitHub](https://github.com/GWeb2015/G-Web-AI-Drafts)  
2. Upload it to `/wp-content/plugins/` on your WordPress site  
3. Activate the plugin through the “Plugins” menu in WordPress  
4. Use the REST API endpoints to create draft posts  

---

## Usage
- Use the REST API endpoint `/wp-json/gweb-ai-drafts/v1/create` (example endpoint, adjust if needed)  
- Include authentication via WordPress user credentials with sufficient permissions  
- Include data for posts:  
  - `title`  
  - `content`  
  - `categories`  
  - `tags`  
  - `featured_image_url`  
  - Yoast SEO fields (`_yoast_wpseo_title`, `_yoast_wpseo_metadesc`, etc.)  
- Supports **bulk creation** by sending multiple post objects in the API payload  

> Note: This plugin is designed for demonstration and internal automation purposes. Future updates may include an admin UI for easier configuration.  

---

## Requirements
- WordPress 6.0+  
- PHP 7.4+  
- REST API enabled  
- Yoast SEO plugin installed and active (optional but required for SEO fields)  

---

## Configuration
- Currently, settings (authentication, field mappings) are **handled via REST API requests**  
- Future versions will include an admin settings page for easier configuration of default post fields and bulk operations  

---

## Changelog
**v1.4**  
- Improved bulk creation performance  
- Added support for featured image URLs  
- Enhanced Yoast SEO field integration  

**v1.0**  
- Initial release: create single or multiple draft posts via REST API with Yoast SEO fields, categories, and tags  

---

## License
This plugin is licensed under the **MIT License**. See [LICENSE](LICENSE) for details.  

---

## Contributing
Contributions are welcome! Fork the repository, submit pull requests, or open issues for bug reports and feature suggestions.  
