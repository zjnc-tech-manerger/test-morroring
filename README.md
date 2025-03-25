test
# byconity.github.io

## Developing

This website is powered by [Docusarus](https://docusaurus.io/). We are using version 2.x at the moment.
You are encouraged to understand the basics of Docusaurus first.

Before run the below script, please [install pnpm](https://pnpm.io/installation) first.

```bash
pnpm install # Install NPM dependencies

pnpm start # Start local server, OR

pnpm start -l zh-cn # Start the zh-cn server

pnpm run build # Build the Website
```

## General Folder Structure

```txt
byconity.github.io/
├── community/ # English pages for the community/* routes
│   ├── category-1
│   │   ├── assets/ # Images used in category-1
│   │   ├── _category_.json # Metadata for category-1
│   │   └──doc-1.md
│   ├── become-maintainer.mdx
│   └── community-code-of-conduct.mdx
│
├── docs/ # Latest English docs, use kebab-case
│   ├── category-1
│   │   ├── assets/ # Images used in category-1
│   │   ├── _category_.json # Metadata for category-1
│   │   └──doc-1.md
│   ├── doc-2.md
│   └── doc-3.md
│
├── versioned_docs/
│   └── version-0.2.0 # Version 0.2.0 English docs, use kebab-case
│       ├── category-1
│       │   ├── assets/ # Images used in category-1
│       │   ├── _category_.json # Metadata for category-1
│       │   └──doc-1.md
│       ├── doc-2.md
│       └── doc-3.md
│
├── versioned_sidebars/
│   └── version-0.2.0-sidebars.json # Version 0.2.0 English sidebar
│
├── blog/ # English blogs, use kebab-case
│   ├── 2021-01-01-happy-new-year.md
│   └── 2021-02-14-valentines-day.md
│
├── i18n/
│   └── zh-CN/
│       ├── docusaurus-plugin-content-docs/
│       │   ├── current/ # Latest Chinese docs, use kebab-case
│       │   │   ├── category-1
│       │   │   │   ├── assets/ # Images used in category-1
│       │   │   │   ├── _category_.json # Metadata for category-1
│       │   │   │   └──doc-1.md
│       │   │   ├── doc-2.md
│       │   │   └── doc-3.md
│       │   ├── current.json # Latest Chinese sidebar
│       │   │
│       │   ├── version-0.2.0/ # Version 0.2.0 Chinese docs, use kebab-case
│       │   │   ├── category-1
│       │   │   │   ├── assets/ # Images used in category-1
│       │   │   │   ├── _category_.json # Metadata for category-1
│       │   │   │   └──doc-1.md
│       │   │   ├── doc-2.md
│       │   │   └── doc-3.md
│       │   └── version-0.2.0.json # Version 0.2.0 Chinese sidebar
│       │
│       ├── docusaurus-plugin-content-docs-community/ # Chinese commuity pages, use kebab-case
│       │   ├── become-maintainer.mdx
│       │   └── community-code-of-conduct.mdx
│       │
│       └── docusaurus-plugin-content-blog/
│           └── current/ # Chinese blogs, use kebab-case
│               ├── 2021-01-01-happy-new-year.md
│               └── 2021-02-14-valentines-day.md
│
├── src/ # Website source code
└── static/
    └── img/
        └── dbyconity-social-card # Opengraph Social Card
```

## For Writers

### Docs

#### File Location

| Version | Language |                                                          Path                                                          |
| :-----: | :------: | :--------------------------------------------------------------------------------------------------------------------: |
| Latest  |    en    |                                                    [docs/](./docs/)                                                    |
| Latest  |  zh-cn   |       [i18n/zh-cn/docusaurus-plugin-content-docs/current/](./i18n/zh-cn/docusaurus-plugin-content-docs/current/)       |
|  0.2.0  |    en    |                            [versioned_docs/version-0.2.0/](./versioned_docs/version-0.2.0/)                            |
|  0.2.0  |  zh-cn   | [i18n/zh-cn/docusaurus-plugin-content-docs/version-0.2.0/](./i18n/zh-cn/docusaurus-plugin-content-docs/version-0.2.0/) |

#### Editing Docs

- Learn the basics at https://docusaurus.io/docs/2.x/create-doc.
- Docs front matters at https://docusaurus.io/docs/2.x/api/plugins/@docusaurus/plugin-content-docs#markdown-front-matter.

### Blog Posts

#### File Location

| Language |                                                    Path                                                    |
| :------: | :--------------------------------------------------------------------------------------------------------: |
|    en    |                                              [blog/](./blog/)                                              |
|  zh-cn   | [i18n/zh-cn/docusaurus-plugin-content-blog/current/](./i18n/zh-cn/docusaurus-plugin-content-blog/current/) |

#### Editing Blog Posts

- Learn the basics at https://docusaurus.io/docs/blog.
- Blog front matters at https://docusaurus.io/docs/api/plugins/@docusaurus/plugin-content-blog#markdown-front-matter
