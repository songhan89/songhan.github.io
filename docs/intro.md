---
sidebar_position: 1
---

# Tutorial Intro

Let's discover **Docusaurus in less than 5 minutes**.

## Getting Started

Get started by **creating a new site**.

Or **try Docusaurus immediately** with **[docusaurus.new](https://docusaurus.new)**.

## Generate a new site

Generate a new Docusaurus site using the **classic template**:

```bash
npm init docusaurus@latest my-website classic
```

## Start your site

Run the development server:

```bash
cd my-website
npm run start
```

## Drawing Diagrams with Mermaid

Docusaurus supports diagrams and flowcharts using [Mermaid](https://mermaid.js.org/). To enable Mermaid, install the plugin:

```bash
npm install @docusaurus/theme-mermaid
```

Then update your `docusaurus.config.js`:

```js
module.exports = {
    // ...
    themes: ['@docusaurus/theme-mermaid'],
    markdown: {
        mermaid: true,
    },
    // ...
};
```

Now you can create diagrams using mermaid code blocks:

```mermaid
graph TD;
        A-->B;
        A-->C;
        B-->D;
        C-->D;
```

You can also create flowcharts, sequence diagrams, and more:

```mermaid
sequenceDiagram
        participant Alice
        participant Bob
        Alice->>John: Hello John, how are you?
        loop Healthcheck
                John->>John: Fight against hypochondria
        end
        Note right of John: Rational thoughts <br/>prevail!
        John-->>Alice: Great!
        John->>Bob: How about you?
        Bob-->>John: Jolly good!
```


Your site starts at `http://localhost:3000`.
