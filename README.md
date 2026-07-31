# PortfolioGit

## MCP servers

This repo has a project-scoped MCP config (`.mcp.json`) for local development:

- **vcvrack** — connects to the [VCV Rack MCP Server plugin](https://github.com/Neural-Harmonics/vcv-rack-plugin-mcp-server) (subscribe to "MCP Server" by Neural Harmonics in VCV Rack's Library, or install from GitHub Releases). With VCV Rack running and the module's server enabled, it exposes `http://127.0.0.1:2600/mcp`, letting an MCP client inspect/build patches, manage modules and cabling, read/set parameters, and save/load `.vcv` files. Local-only, no auth — only works when Claude Code runs on the same machine as VCV Rack.