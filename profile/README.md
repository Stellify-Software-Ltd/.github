# Stellify - AI-Native Code Composition Platform

From the team at Stellify Software Ltd. comes Stellify, a web-based AI IDE that generates structured code, imports PHP & JS projects, and exports clean, production-ready codebases — so you can ship faster and own everything.

---

## What is Stellify?

Stellify is a convergence platform that fundamentally changes how AI writes code. Instead of generating code character-by-character as raw text, Stellify stores code as structured JSON in a database, enabling AI to compose applications from curated, proven building blocks.

Traditional AI coding tools regenerate the same solutions thousands of times—each with subtle variations, bugs, and inconsistencies. Stellify eliminates this by having AI reference and compose existing, validated code patterns.

---

## Key Features

### Structured Code Storage

- **Code as structured data** — Methods, statements, and clauses stored as JSON, not text files
- **Hash-based deduplication** — Identical code detected and reused automatically
- **Granular editing** — Modify individual statements without parsing entire files
- **AI-friendly format** — Structured data is easier for AI to understand and manipulate precisely

### AI Integration via MCP

- 40+ MCP tools for seamless AI assistant integration
- Works with Claude Desktop, Claude Code CLI, and any MCP-compatible client
- AI operates on semantic units (methods, statements, elements) rather than raw text
- Structured guardrails keep AI in check—only valid operations allowed, syntax validated at every step

### Full-Stack Development

- **Laravel/PHP backend** — Controllers, models, middleware, services
- **Vue.js frontend** — Single File Components with reactive state
- **Visual Interface Builder** — 15+ element types for UI composition
- **Code Editor** — VSCode-like experience for backend logic

### Unified Platform

Everything in one place:

- Interface design
- Backend code
- Version control (Git-like branching without external tools)
- Asset management
- Export & deployment
- AI integration

### Zero Lock-In

- **Export production-ready code** — Standard Laravel/Vue applications
- **Deploy anywhere PHP runs**
- **Full ownership of your code**

---

## How It Works

### Traditional AI Flow

```
User: "Add a login function"
  → AI generates text: "function login($email..."
  → Hope it's syntactically correct
  → Hope it matches existing patterns
  → Hope imports are handled
```

### Stellify AI Flow

```
User: "Add a login function"
  → AI calls create_method() with validated parameters
  → System validates method signature
  → AI calls add_method_body() with parsed code
  → Dependencies auto-resolved
  → Syntax validated at every step
  → ✅ Working code guaranteed
```

---

## Why Stellify?

| Traditional Approach | Stellify Approach |
|----------------------|-------------------|
| AI guesses at structure | AI operates on semantic units |
| Syntax errors possible | Syntax validated at every step |
| Inconsistent patterns | Consistent structure enforced |
| Missing imports/dependencies | Dependencies auto-resolved |
| Hard to detect duplicates | Hash-based deduplication |
| Scattered across tools | Unified platform |

---

## Current Capabilities

- ✅ Build full-stack web applications (Laravel + Vue)
- ✅ Visual interface builder with 15+ element types
- ✅ Code editor for PHP methods and statements
- ✅ MCP server for AI assistants
- ✅ HTML → Elements conversion in single API call
- ✅ Vue 3 SFC bundling via esbuild (~50ms builds)
- ✅ Real-time AI-to-browser broadcasting via WebSockets
- ✅ Execution benchmarking with timing, memory, and query metrics
- ✅ Version control with branching and merging
- ✅ 65+ global Laravel framework classes available
- ✅ Code import from existing PHP/JavaScript files

---

## Open Source Components

- **[stellify-mcp](https://github.com/Stellify-Software-Ltd/stellify-mcp)** — MCP server for AI integration
- **[stellify-laravel](https://github.com/Stellify-Software-Ltd/stellify-laravel)** — Laravel project importer
- **[stellify-bundler-service](https://github.com/Stellify-Software-Ltd/stellify-bundler-service)** — JavaScript bundling service

---

## Get Started

1. Install the MCP server:
   ```bash
   npm install -g @stellify/mcp-server
   ```
2. Configure with your Stellify API token
3. Connect Claude Desktop or Claude Code
4. Start building with AI

---

## Links

- **Website:** [stellisoft.com](https://stellisoft.com)
- **Documentation:** [docs](https://stellisoft.com/stellify/documentation)
- **GitHub:** [Stellify-Software-Ltd](https://github.com/Stellify-Software-Ltd)

---

**Stellify** — where AI meets battle-tested code to build better software.
