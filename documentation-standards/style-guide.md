# Technical Documentation Style Guide

## 1. Purpose

This style guide defines the writing, formatting, terminology, and structural standards used throughout this technical writing portfolio.

Its purpose is to maintain consistency across documentation projects, improve readability, and ensure that information is presented clearly to the intended audience.

These guidelines apply to all documentation within this repository, including:

- Installation guides
- API references
- Architecture documentation
- User guides
- Troubleshooting guides
- Glossaries
- Technical overviews

## 2. Writing Principles

All documentation should follow these core principles.

| Principle | Guideline |
|---|---|
| Clarity | Use straightforward language and explain complex concepts clearly. |
| Accuracy | Verify technical information against reliable sources or actual system behaviour. |
| Consistency | Use the same terminology, formatting, and writing style throughout. |
| Conciseness | Include relevant information without unnecessary repetition. |
| Usability | Organise content so readers can quickly find what they need. |
| Accessibility | Use descriptive headings, meaningful links, and readable formatting. |

## 3. Tone and Language

### 3.1 Writing Tone

The preferred tone is:

- Professional
- Clear
- Neutral
- Helpful
- Direct
- User-focused

Documentation should sound informative rather than conversational or promotional.

### 3.2 Sentence Structure

Use short and direct sentences wherever possible.

**Preferred:**

> Open the application and select the Login option. Enter your registered email address and password.

**Avoid:**

> In order to gain access to the application, users will need to navigate to the login section, where they can proceed to enter the necessary credentials.

### 3.3 Active Voice

Use active voice when it makes instructions easier to understand.

**Preferred:**

> Select Save to update the record.

**Avoid:**

> The record should be updated by selecting Save.

Passive voice may be used when the person performing an action is unknown or unimportant.

### 3.4 Point of View

Use second-person language ("you") when providing instructions to end users.

Use neutral third-person language when describing system functionality, architecture, or technical concepts.

Avoid unnecessary use of first-person language in procedural documentation.

## 4. Document Structure

Documents should follow a consistent hierarchy.

### 4.1 Headings

Use Markdown heading levels according to their purpose.

| Markdown | Usage |
|---|---|
| `#` | Main document title |
| `##` | Main sections |
| `###` | Subsections |
| `####` | Smaller subsections, when necessary |

Example:

```markdown
# Installation Guide

## Prerequisites

## Installation Steps

### Configure the Database

### Start the Backend

## Verification
```

Guidelines:

- Use one main `#` heading per document.
- Keep headings descriptive and meaningful.
- Maintain a logical heading hierarchy.
- Do not skip heading levels unnecessarily.
- Use sentence case for headings.

### 4.2 Paragraphs

- Keep paragraphs focused on one main idea.
- Avoid unnecessarily long blocks of text.
- Use lists when presenting multiple related items.
- Separate different procedures into distinct sections.

### 4.3 Lists

Use numbered lists for sequential instructions.

Example:

```markdown
1. Open the project directory.
2. Install the required dependencies.
3. Configure the environment variables.
4. Start the application.
```

Use bullet points for non-sequential information.

Example:

```markdown
- React
- ASP.NET Core
- PostgreSQL
- Entity Framework Core
```

## 5. Formatting Standards

### 5.1 Bold Text

Use bold formatting for:

- Important labels
- Interface elements when clarity benefits
- Key warnings or important information
- Short introductory labels

Example:

> **Note:** Ensure the database is running before starting the backend.

Avoid excessive bold formatting.

### 5.2 Italics

Use italics sparingly for emphasis or for introducing a term where appropriate.

### 5.3 Code Formatting

Use inline code formatting for:

- File names: `appsettings.json`
- Folder names: `Controllers/`
- Commands: `dotnet restore`
- Variables: `connectionString`
- API paths: `/api/users`
- Database names: `SastagramDb`

Use fenced code blocks for longer code examples and commands.

Specify the language where possible.

Example:

```bash
dotnet restore
dotnet run
```

### 5.4 Tables

Use tables to organise information that benefits from direct comparison.

Examples include:

- API endpoint summaries
- Configuration variables
- Technology stacks
- Error descriptions and resolutions

Keep tables readable and avoid placing long paragraphs inside table cells.

### 5.5 Links

- Use descriptive link text.
- Link to relevant documentation or supporting resources.
- Avoid vague labels such as "click here".
- Check that links work before publishing.

Preferred:

```markdown
Refer to the [Installation Guide](installation.md).
```

Avoid:

```markdown
Click [here](installation.md).
```

## 6. Instructions and Procedures

Procedural documentation should help readers complete a task successfully.

Each procedure should include the following where relevant:

1. **Purpose:** Explain what the procedure accomplishes.
2. **Prerequisites:** Identify anything the reader needs before starting.
3. **Steps:** Present instructions in the correct sequence.
4. **Expected result:** Explain what should happen after completion.
5. **Troubleshooting:** Refer readers to relevant solutions if something goes wrong.

### Instruction Writing Rules

- Start each step with an action verb.
- Keep each step focused on one main action.
- Include the location of relevant settings, files, or controls.
- Explain expected results when they are not obvious.
- Do not omit important prerequisites.
- Do not assume the reader knows the system.

Example:

```markdown
## Starting the Backend

Before starting, ensure PostgreSQL is running and the
database connection is configured.

1. Open the backend project directory.
2. Open a terminal.
3. Run the following command:

   `dotnet run`

4. Check the terminal output for the application startup message.

**Expected result:** The backend application starts successfully
and listens on its configured address.
```

## 7. Technical Terminology

### 7.1 Consistent Terminology

Use the same term for the same concept throughout a document.

For example:

| Preferred Term | Avoid Switching Between |
|---|---|
| User account | Account, profile, user record (when referring to the same concept) |
| Database | DB, data store (unless technically distinct) |
| API endpoint | Route, URL (when referring specifically to an endpoint) |
| Patient record | Patient profile, patient file (when referring to the same concept) |

Different terms may be appropriate when they have different technical meanings.

### 7.2 Acronyms

- Write the full term the first time it appears.
- Introduce the acronym in brackets.
- Use the acronym consistently afterwards.

Example:

> Representational State Transfer (REST) is an architectural style used in web APIs.

Common technical acronyms may be used without expansion when the intended audience is expected to know them.

### 7.3 Product and Technology Names

Use official spelling and capitalisation.

Examples:

- OpenMRS
- PostgreSQL
- ASP.NET Core
- GitHub
- React
- REST API
- Visual Studio Code

Do not invent product names or alter official technology terminology.

## 8. Warnings, Notes, and Important Information

Use clear labels to distinguish different types of information.

**Note:** Provides additional information that may help the reader.

**Important:** Highlights information necessary for successful completion of a task.

**Warning:** Identifies a risk that could result in data loss, security issues, or unintended behaviour.

Example:

> **Warning:** Do not commit passwords, API keys, or database credentials to a public repository.

Use warnings only when a genuine risk exists.

## 9. Screenshots and Diagrams

Visual elements should support the written explanation rather than replace it.

### Screenshots

- Use screenshots that are relevant to the described procedure.
- Ensure text and interface elements are readable.
- Remove personal, confidential, or sensitive information.
- Use captions to explain what the screenshot demonstrates.
- Keep screenshots consistent in size and presentation where practical.
- Verify that screenshots represent the correct application version.

### Diagrams

Use diagrams when they help explain:

- System architecture
- Application components
- Data flow
- User workflows
- API interactions

Every diagram should have a descriptive title and, where necessary, a short explanation.

## 10. API Documentation Standards

API documentation should present information consistently.

Where applicable, include:

| Field | Description |
|---|---|
| Endpoint | API path |
| Method | HTTP request method |
| Purpose | What the endpoint does |
| Authentication | Required authentication |
| Parameters | Required and optional inputs |
| Request Body | Expected request structure |
| Response | Expected response structure |
| Status Codes | Relevant HTTP response codes |

Example:

```markdown
### GET /api/users

**Purpose:** Retrieves user information.

**Method:** GET

**Authentication:** Describe the actual authentication
requirements for this endpoint.

**Response:** Document the response structure returned
by the implemented API.
```

Only document endpoints, request fields, and response behaviour that are supported by the actual implementation or a reliable API specification.

## 11. Troubleshooting Documentation Standards

Troubleshooting entries should help readers identify and resolve issues.

Use the following structure:

```markdown
### Issue: [Short description]

**Symptoms:**

Describe what the user experiences.

**Possible Cause:**

Explain the likely reason for the issue.

**Resolution:**

1. Provide the first troubleshooting step.
2. Provide the next step.
3. Explain how to verify the fix.

**Expected Result:**

Describe the expected outcome.
```

Guidelines:

- Describe symptoms clearly.
- Separate confirmed causes from possible causes.
- Provide actionable solutions.
- Include commands or examples when useful.
- Avoid recommending destructive actions without explaining the risk.

## 12. Source and Reference Standards

Technical information should be supported by reliable sources.

Preferred sources include:

- Official product documentation
- Official developer documentation
- API specifications
- Relevant technical standards
- Authoritative government or regulatory resources

When using external sources:

- Include descriptive links.
- Record relevant source names and access details where appropriate.
- Distinguish original research from sourced information.
- Avoid presenting assumptions as verified product functionality.
- Check that references are relevant to the product version being documented.

## 13. Accessibility and Readability

Documentation should be easy to navigate and understand.

Guidelines:

- Use descriptive headings.
- Use meaningful link text.
- Provide alternative text for informative images.
- Do not rely on colour alone to communicate meaning.
- Use tables only when they improve comprehension.
- Keep code examples readable.
- Use consistent formatting throughout the repository.

## 14. Review and Quality Checklist

Before publishing or updating a document, review it against this checklist.

### Content and Accuracy

- [ ] Information is relevant to the document's purpose.
- [ ] Technical details have been checked against reliable sources.
- [ ] Assumptions and limitations are identified.
- [ ] Instructions are complete and logically ordered.
- [ ] Examples match the described system.

### Writing and Structure

- [ ] Headings follow a logical hierarchy.
- [ ] Language is clear and concise.
- [ ] Terminology is consistent.
- [ ] Grammar and spelling have been checked.
- [ ] Repeated or unnecessary information has been removed.

### Formatting and Navigation

- [ ] Markdown formatting is consistent.
- [ ] Code blocks specify the appropriate language.
- [ ] Tables are readable.
- [ ] Links work correctly.
- [ ] Screenshots and diagrams are relevant and readable.

### Security and Publication

- [ ] No passwords or API keys are included.
- [ ] No confidential or personal information is exposed.
- [ ] Screenshots have been reviewed for sensitive information.
- [ ] Sources and references are included where required.

## 15. Maintenance

This style guide should be reviewed as the portfolio grows.

New documentation should follow these standards. Existing documents should be updated when changes are needed to improve accuracy, readability, consistency, or usability.

The objective is to maintain a professional and consistent documentation experience across all projects in this portfolio.