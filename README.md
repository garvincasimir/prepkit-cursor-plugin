# PrepKit for Cursor

This repository contains an Agent Plugins 1.0 package for Cursor. Add it through Cursor's supported plugin installation flow. A public marketplace listing is separate from this repository.

For local development, clone the repository into `~/.cursor/plugins/local/prepkit` and restart Cursor. Check the PrepKit MCP connection in Cursor settings and complete PrepKit authentication when requested. Host installation and tool execution must be checked in your Cursor version.

This package connects an assistant to the PrepKit MCP server at `https://mcp.prepkit.cazimedia.com/mcp`. Your assistant supplies inference through its own account, plan and usage limits. PrepKit does not receive its password or API key.

Sign in to PrepKit when the assistant requests a connection. Review the permissions before approving. Ask your assistant to read `get_kitml_contract`; it returns the complete text-only source schema and a working example. Content submission requires a learner-created upload grant. Submitted kits wait for your review in PrepKit before joining your library.

Text-only assistants can call `validate_kitml_source` and `submit_private_kit_source`. Media packages use the KitML ZIP tools.

To revoke access, open PrepKit, choose **My PrepKits**, then **Create or import**, and disconnect the assistant in the connected list.
