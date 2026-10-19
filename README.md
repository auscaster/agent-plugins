# Auscaster agent plugins

Install first-party plugins for [runx](https://runx.ai), [Sourcey](https://sourcey.com), [Frantic](https://gofrantic.com) and [Ausca](https://ausca.com) in Claude Code or Codex. Each entry points to the product's own public repository, with its current mark, a hosted MCP connection and a scoped skill. Auscaster is the collection name, not a claim that these brands share a legal company.

For Claude Code:

```bash
claude plugin marketplace add auscaster/agent-plugins
claude plugin install runx@auscaster
claude plugin install sourcey@auscaster
claude plugin install frantic@auscaster
claude plugin install ausca@auscaster
```

For Codex, which reads the portable Agent Plugins manifests from the same product repositories:

```bash
codex plugin marketplace add auscaster/agent-plugins
codex plugin add runx@auscaster
codex plugin add sourcey@auscaster
codex plugin add frantic@auscaster
codex plugin add ausca@auscaster
```

The Codex marketplace is a public GitHub distribution route. It is separate from OpenAI's reviewed public Plugins Directory shared with ChatGPT.

Install only the plugins you need. The marketplace adds no background hooks or shell-executing components. The products' own READMEs explain their endpoints, permissions, payment boundaries, documentation and support. An installed plugin does not itself authorize account actions or paid calls.

Nitrosend has its own [Claude connector](https://claude.ai/directory/nitrosend) and [plugin source](https://github.com/nitrosend/claude), published under the Nitrosend identity. This collection does not duplicate that listing.

This repository is a distribution index. Plugin files and licenses live in their official source repositories.
