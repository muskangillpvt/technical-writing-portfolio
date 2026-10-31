# Markdown Documentation Guide

## 1. Introduction

Markdown is a lightweight markup language used to format plain text into structured and readable documents.

It is commonly used for technical documentation, README files, project guides, developer notes, and documentation hosted on platforms such as GitHub.

I use Markdown throughout this portfolio to create consistent, accessible, and easy-to-maintain documentation.

This guide demonstrates the Markdown syntax and formatting conventions used in my documentation projects.

## 2. Headings

Headings organise information into sections and subsections.

Markdown uses the `#` symbol to define heading levels.

| Markdown Syntax | Heading Level | Usage |
|---|---|---|
| `# Heading` | H1 | Main document title |
| `## Heading` | H2 | Main section |
| `### Heading` | H3 | Subsection |
| `#### Heading` | H4 | Smaller subsection |
| `##### Heading` | H5 | Detailed subsection |
| `###### Heading` | H6 | Lowest heading level |

**Example:**

```markdown
# Installation Guide

## Prerequisites

### Required Software

#### Database Configuration
```

**Rendered result:**

# Installation Guide

## Prerequisites

### Required Software

#### Database Configuration

**Best practices:**

- Use one H1 heading per document.
- Keep headings descriptive.
- Maintain a logical heading hierarchy.
- Avoid skipping heading levels unnecessarily.

## 3. Text Formatting

Markdown supports different text styles to highlight important information.

| Formatting | Markdown Syntax | Result |
|---|---|---|
| Bold | `**Important**` | **Important** |
| Italic | `*Example*` | *Example* |
| Bold and italic | `***Important***` | ***Important*** |
| Strikethrough | `~~Removed text~~` | ~~Removed text~~ |
| Inline code | `` `code` `` | `code` |

**Example:**

```markdown
**Important:** Save your configuration before starting the application.

*Note:* The database must be running.

Use `dotnet run` to start the backend.
```

**Rendered result:**

**Important:** Save your configuration before starting the application.

*Note:* The database must be running.

Use `dotnet run` to start the backend.

## 4. Lists

Lists make information easier to scan and understand.

### 4.1 Unordered Lists

Use hyphens (`-`), asterisks (`*`), or plus signs (`+`) to create bullet points.

```markdown
- React
- ASP.NET Core
- PostgreSQL
- Entity Framework Core
```

**Rendered result:**

- React
- ASP.NET Core
- PostgreSQL
- Entity Framework Core

### 4.2 Ordered Lists

Use numbers followed by periods for sequential instructions.

```markdown
1. Open the project directory.
2. Install dependencies.
3. Configure the database.
4. Start the application.
```

**Rendered result:**

1. Open the project directory.
2. Install dependencies.
3. Configure the database.
4. Start the application.

### 4.3 Nested Lists

Indent lists to create sub-items.

```markdown
- Backend
  - Controllers
  - Services
  - Models
- Frontend
  - Components
  - Pages
  - Services
```

**Rendered result:**

- Backend
  - Controllers
  - Services
  - Models
- Frontend
  - Components
  - Pages
  - Services

## 5. Links

Links connect documents, external resources, and related information.

### 5.1 External Links

```markdown
[GitHub](https://github.com)
```

**Rendered result:** [GitHub](https://github.com)

### 5.2 Internal Links

Internal links connect Markdown files within the same repository.

```markdown
[Installation Guide](../projects/sastagram/installation.md)
```

**Rendered result:** [Installation Guide](../projects/sastagram/installation.md)

### 5.3 Links to Sections

Use heading anchors to link directly to a section.

```markdown
[View Prerequisites](#prerequisites)
```

**Best practices:**

- Use descriptive link text.
- Check that links point to the correct location.
- Prefer relative paths for links within the repository.
- Avoid vague phrases such as "click here".

## 6. Images

Images can be included to explain interfaces, workflows, and system components.

**Syntax:**

```markdown
![Alternative text](../assets/screenshots/dashboard.png)
```

**Example:**

```markdown
![Application Dashboard](../assets/screenshots/dashboard.png)
```

The alternative text describes the image for readers who cannot see it and for assistive technologies.

**Best practices:**

- Use descriptive alternative text.
- Keep images relevant to the surrounding content.
- Use readable screenshots.
- Remove sensitive information before publishing.
- Use relative paths for repository images.

## 7. Code Blocks

Code blocks are useful for displaying commands, configuration examples, and source code.

### 7.1 Inline Code

Use single backticks for short code references.

```markdown
Run `dotnet restore` to install the project dependencies.
```

**Rendered result:**

Run `dotnet restore` to install the project dependencies.

### 7.2 Fenced Code Blocks

Use three backticks before and after a code block.

Specify the programming language after the opening backticks to enable syntax highlighting.

**Example:**

````markdown
```bash
dotnet restore
dotnet run
```
````

**Rendered result:**

```bash
dotnet restore
dotnet run
```

### 7.3 JSON Example

````markdown
```json
{
  "name": "Sastagram",
  "environment": "development"
}
```
````

**Rendered result:**

```json
{
  "name": "Sastagram",
  "environment": "development"
}
```

### Common Language Identifiers

| Language | Identifier |
|---|---|
| JavaScript | `javascript` |
| TypeScript | `typescript` |
| C# | `csharp` |
| Python | `python` |
| SQL | `sql` |
| JSON | `json` |
| HTML | `html` |
| CSS | `css` |
| Bash | `bash` |
| YAML | `yaml` |
| XML | `xml` |

## 8. Tables

Tables organise structured information into rows and columns.

**Syntax:**

```markdown
| Component | Technology |
|---|---|
| Frontend | React |
| Backend | ASP.NET Core |
| Database | PostgreSQL |
```

**Rendered result:**

| Component | Technology |
|---|---|
| Frontend | React |
| Backend | ASP.NET Core |
| Database | PostgreSQL |

### 8.1 Text Alignment

Colons control text alignment.

```markdown
| Left | Centre | Right |
|:---|:---:|---:|
| A | B | C |
| D | E | F |
```

**Rendered result:**

| Left | Centre | Right |
|:---|:---:|---:|
| A | B | C |
| D | E | F |

Use tables for concise comparisons, configuration details, and API summaries. Avoid using them for long paragraphs.

## 9. Blockquotes

Blockquotes highlight notes, references, or important information.

**Syntax:**

```markdown
> This is an example of a blockquote.
```

**Rendered result:**

> This is an example of a blockquote.

Blockquotes can also contain multiple paragraphs.

```markdown
> **Note:** Ensure the database is running.
>
> Start the backend after confirming the database connection.
```

## 10. Horizontal Rules

Horizontal rules separate major sections of a document.

**Syntax:**

```markdown
---
```

**Rendered result:**

---

Use horizontal rules sparingly to separate distinct content sections.

## 11. Task Lists and Checkboxes

GitHub Markdown supports interactive task-list checkboxes.

**Syntax:**

```markdown
- [x] Create the repository
- [x] Write the README
- [ ] Add screenshots
- [ ] Review documentation
```

**Rendered result:**

- [x] Create the repository
- [x] Write the README
- [ ] Add screenshots
- [ ] Review documentation

Task lists are useful for:

- Project progress tracking
- Documentation review checklists
- Installation requirements
- Quality assurance activities

## 12. Escaping Markdown Characters

Sometimes Markdown characters need to be displayed as normal text instead of being interpreted as formatting.

Use a backslash (`\`) before a special character.

**Example:**

```markdown
\*This is not italic text\*
```

**Rendered result:**

\*This is not italic text\*

This is useful when documenting Markdown syntax itself.

## 13. File and Folder References

When documenting software projects, use inline code formatting for file and folder names.

**Example:**

```markdown
The application configuration is stored in `appsettings.json`.

The API controllers are located in the `Controllers/` directory.
```

**Rendered result:**

The application configuration is stored in `appsettings.json`.

The API controllers are located in the `Controllers/` directory.

## 14. Recommended Documentation Structure

A typical Markdown documentation file can follow this structure:

```markdown
# Document Title

## Introduction

Briefly explain the purpose of the document.

## Prerequisites

List anything required before starting.

## Instructions

1. Complete the first step.
2. Complete the second step.
3. Verify the result.

## Troubleshooting

Explain common issues and their solutions.

## References

Include relevant resources and links.
```

The structure should be adapted to the document's purpose rather than applied rigidly to every file.

## 15. GitHub Markdown Considerations

GitHub supports standard Markdown as well as additional GitHub Flavored Markdown (GFM) features.

Some useful GitHub features include:

- Task lists
- Tables
- Automatic URL linking
- Strikethrough text
- Mentioning users and referencing issues or pull requests
- Syntax highlighting in code blocks

Markdown rendering can vary between platforms. Always preview documents on the platform where they will be published.

## 16. Markdown Quality Checklist

Before publishing a Markdown document, review the following:

### Structure

- [ ] The document has a clear title.
- [ ] Headings follow a logical hierarchy.
- [ ] Sections are organised in a meaningful order.
- [ ] Paragraphs are easy to read.

### Formatting

- [ ] Bold and italic formatting is used consistently.
- [ ] Lists are formatted correctly.
- [ ] Tables are aligned and readable.
- [ ] Code blocks specify the appropriate language.
- [ ] Links and image paths are correct.

### Accessibility

- [ ] Images include descriptive alternative text.
- [ ] Links have meaningful labels.
- [ ] Information is not communicated through colour alone.
- [ ] Tables are used appropriately.

### Final Review

- [ ] Spelling and grammar have been checked.
- [ ] No unnecessary formatting has been used.
- [ ] The document has been previewed on GitHub.
- [ ] No sensitive information is exposed.

## 17. References

- [GitHub Flavored Markdown Specification](https://github.github.com/gfm/)
- [GitHub: Basic Writing and Formatting Syntax](https://docs.github.com/en/get-started/writing-on-github)
- [Markdown Guide](https://www.markdownguide.org/)

---

**Document purpose:** This guide serves as a practical reference for the Markdown syntax and formatting conventions used throughout my technical writing portfolio.