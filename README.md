# Articul8 Style Guide
Example of Markdown-based style guide for product, API, and release note documentation. 

Generally speaking, this will align with the [Github Basic Writing and Formatting Guide](https://docs.github.com/en/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax) syntax and guidelines.

Examples of the **Product** and **Release Note** types will be available as additional files in this project.

## Product Documentation

1. Documentation titles will use H1 (# Title)
2. An "Introduction" will follow using H2 (## Introduction)
3. The remainder of the content will use H2, H3, and H4 (####) headings for subsequent sections.
4. These articles and items will be hosted in GitHub and published via GitHub Pages to a MKDocs site (pending final publication tooling decision).
5. This documentation will be published as a documentation hub as a sub-domain of the Articul8 home page, eg "docs.articul8.ai", "wiki.articul8.ai", or similar.
   - Additional forms of technical documentation, such as API reference, release notes, troubleshooting guides, etc, should all be accessible from a header navigation panel, while being independently accessible via "docs.articul8.ai/API" or similar. 

### Specific Formatting and Syntax

1. Markdown content, including prose, code, and hosted media, will follow the Github-flavored Markdown (GFM) standards described [here](https://docs.github.com/en/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax).

## API Documentation

1. We will use OpenAPI standards, which will help with automatic API doc generation.
2. These generated API Docs will contain the following:
   - Introduction, including prerequisites, how to access an API key, support contact information, etc
   - The API Endpoint
       - if there are sub-endpoints, they will be nested below
   - Authentication instructions and requirements
   - List of potential HTTP responses, with explanations.
   - The required (and optional) parameters, with explanations. 
   - A sample request body
   - A request example in multiple formats (at minimum, cURL and Python)
3. Individual endpoints will be accessible via direct URL link
4. These API docs should be hosted in a similar place to the public-facing documentation hub.
   - eg "docs.articul8.ai/API" or similar

## Release Notes

1. **Release Notes** will be titled with an H1 section, which will include, at minimum:
   - a release version in the form of `v.majorVersion.minorVersion`, eg `v1.0`
   - a product name, eg "Articul8 Essential"
2. **Release Notes** will be timestamped.
3. They will contain H2 sections for "New Changes", "Bugfixes", and any other high-level classifications
4. They will contain H3 sections based on relevant changes made to a given part of the product:
  - eg "ModelMesh (tm)", "API", "Infrastructure", etc
4. They will contain inline hyperlinks to relevant documentation, where available
5. If there are no updates to provide for a given section, they will NOT be included in the release note. 
