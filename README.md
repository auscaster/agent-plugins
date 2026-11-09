# auscaster agent plugins

Install first-party plugins for [runx](https://runx.ai), [Sourcey](https://sourcey.com), [Frantic](https://gofrantic.com), [Ausca](https://ausca.com), [Silvertongue](https://github.com/auscaster/silvertongue) and [UGT](https://usegeekthing.com) in Claude Code or Codex. Each entry points to the product's own public repository, with its current mark, an MCP connection and a scoped skill: a hosted one, or for UGT, which runs on your computer, `ugt mcp` from UGT itself. auscaster is the collection name, not a claim that these brands share a legal company.

For Claude Code:

```bash
claude plugin marketplace add auscaster/agent-plugins
claude plugin install runx@auscaster
claude plugin install sourcey@auscaster
claude plugin install frantic@auscaster
claude plugin install ausca@auscaster
claude plugin install silvertongue@auscaster
claude plugin install ugt@auscaster
```

For Codex, which reads the portable Agent Plugins manifests from the same product repositories:

```bash
codex plugin marketplace add auscaster/agent-plugins
codex plugin add runx@auscaster
codex plugin add sourcey@auscaster
codex plugin add frantic@auscaster
codex plugin add ausca@auscaster
codex plugin add silvertongue@auscaster
codex plugin add ugt@auscaster
```

The Codex marketplace is a public GitHub distribution route. It is separate from OpenAI's reviewed public Plugins Directory shared with ChatGPT.

Install only the plugins you need. The marketplace adds no background hooks. UGT's plugin starts `ugt mcp`, UGT's own server on your computer, so install UGT first (`curl -fsSL https://usegeekthing.com/install | sh`, or `irm https://usegeekthing.com/install.ps1 | iex` on Windows); the others connect to hosted servers. The products' own READMEs explain their endpoints, permissions, payment boundaries, documentation and support. An installed plugin does not itself authorize account actions or paid calls.

Nitrosend has its own [Claude connector](https://claude.ai/directory/nitrosend) and [plugin source](https://github.com/nitrosend/claude), published under the Nitrosend identity. This collection does not duplicate that listing.

This repository is a distribution index. Plugin files and licenses live in their official source repositories.
