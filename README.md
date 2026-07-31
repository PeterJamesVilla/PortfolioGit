# PortfolioGit

## MCP servers

This repo has a project-scoped MCP config (`.mcp.json`) for local development:

- **vcvrack** — connects to the [VCV Rack MCP Server plugin](https://github.com/Neural-Harmonics/vcv-rack-plugin-mcp-server) (`NeuralHarmonics`, MIT-licensed, free). Not in VCV Rack's official Library — install manually: download the `.zip` for your OS from the [Releases page](https://github.com/Neural-Harmonics/vcv-rack-plugin/releases), extract the `NeuralHarmonics` folder into your Rack2 plugins directory (`~/Library/Application Support/Rack2/plugins-mac-arm64/` or `plugins-mac-x64/` on macOS, `~/.local/share/Rack2/plugins-lin-x64/` on Linux), then restart Rack and add the module from the browser under Utility. With VCV Rack running and the module's server enabled, it exposes `http://127.0.0.1:2600/mcp`, letting an MCP client inspect/build patches, manage modules and cabling, read/set parameters, and save/load `.vcv` files. Local-only, no auth — only works when Claude Code runs on the same machine as VCV Rack.