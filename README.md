# XRepublic Documentation Site

A Hugo-based documentation site for the XRepublic project - a virtual parliament system for collaborative decision-making and deliberative democracy.

## About XRepublic

The XRepublic is a computer-mediated deliberation process designed to fundamentally change how people share ideas for collaborative decision making. It serves as a virtual parliament utilizing web-based technology to make deliberative processes available to distributed groups connected by networked computers.

**Live Site:** https://xrepublic.info/

## Project Structure

This is a Hugo static site using the Docsy theme:

```
├── config/           # Hugo configuration files
├── content/          # Markdown content files
│   ├── about/        # About pages
│   ├── docs/         # Documentation content
│   │   ├── introduction/
│   │   ├── reference/
│   │   └── abuse/
│   ├── glossary.md
│   └── friends.md
├── themes/           # Hugo themes (Docsy)
├── public/           # Generated static site
├── assets/           # Site assets
└── resources/        # Hugo resources
```

## Development

### Prerequisites

- [Hugo](https://gohugo.io/installation/) (Extended version)
- [Node.js](https://nodejs.org/) and npm (for PostCSS processing)

### Setup

1. Clone the repository:
   ```bash
   git clone <repository-url>
   cd xrepublic-info
   ```

2. Install npm dependencies:
   ```bash
   npm install
   ```

3. Run the development server:
   ```bash
   hugo server -D
   ```

4. Open http://localhost:1313 in your browser

### Building

To build the site for production:

```bash
hugo
```

The generated site will be in the `public/` directory.

## Deployment

The site is configured to deploy to AWS S3 with CloudFront CDN. Configuration is in `config/_default/config.toml`:

- **S3 Bucket:** s3://www.mdcbowen.info
- **CloudFront Distribution:** E2H153ADGJ7YZX
- **Region:** us-west-2

To deploy:

```bash
hugo deploy
```

## Theme

This site uses the [Docsy](https://www.docsy.dev/) Hugo theme, which provides:

- Clean documentation layout
- Search functionality
- Multi-language support
- Responsive design
- Navigation structure

## Content Management

- Content is written in Markdown and stored in the `content/` directory
- Front matter in YAML format controls page metadata
- The site supports taxonomies: tags, categories, authors, and series

## Contributing

1. Create content in the appropriate `content/` subdirectory
2. Use Markdown format with YAML front matter
3. Test locally with `hugo server`
4. Submit pull requests for review

## Links and Resources

### Project Resources
- [XR Civics PDF](https://mdcb-public-data.s3-us-west-2.amazonaws.com/xr/XR%20Civics%20V01.pdf)
- [Why Can't We Be Citizens?](https://mdcbowen.substack.com/p/why-cant-we-be-citizens)
- [Barriers to Agreement](https://tessellations.substack.com/p/xr-barriers-to-agreement)
- [The XRepublic System](https://www.mdcbowen.org/p5/xrstatic/index.htm)

### Technical Documentation
- [Hugo Documentation](https://gohugo.io/documentation/)
- [Docsy Theme Documentation](https://www.docsy.dev/docs/)

## License

[License information to be added]

## Contact

[Contact information to be added]