# AbuHashem Website

This repository contains the source code for the AbuHashem website, built using the [Hugo](https://gohugo.io/) static site generator and the [Congo](https://github.com/jpanther/congo) theme.

## Overview

The website serves as a personal blog or platform for sharing content, primarily in Arabic, based on the current structure.

## Getting Started

To run this project locally, you'll need to have [Hugo](https://gohugo.io/installation/) installed.

1.  **Clone the repository:**
    ```bash
    git clone <repository-url>
    cd AbuHashem
    ```
    *(Replace `<repository-url>` with the actual URL of your Git repository)*

2.  **Initialize Submodules:** The theme is included as a Git submodule. Initialize it:
    ```bash
    git submodule update --init --recursive
    ```

3.  **Run the Hugo server:**
    ```bash
    hugo server
    ```
    This command builds the site and starts a local server, typically accessible at `http://localhost:1313/`. The site will automatically reload when you make changes to the content or configuration.

## Creating Content

New content (like blog posts) can be created using the Hugo CLI:

```bash
hugo new content posts/my-new-post.md
```

This will create a new Markdown file in the `content/posts/` directory based on the default archetype (`archetypes/default.md`). Edit this file to add your content.

## Building for Production

To build the static site files for deployment:

```bash
hugo
```

This command generates the static website files in the `public/` directory. These files can then be deployed to any static web hosting service.

## Theme

This project uses the [Congo](https://github.com/jpanther/congo) theme, located in the `themes/congo` directory as a submodule. Refer to the theme's documentation for customization options.

## Configuration

Main configuration files are located in the `config/_default/` directory:
*   `hugo.toml`: Core Hugo settings.
*   `params.toml`: Theme-specific parameters.
*   `menus.ar.toml`: Menu configuration for the Arabic language.
*   `languages.ar.toml`: Language-specific settings for Arabic.
