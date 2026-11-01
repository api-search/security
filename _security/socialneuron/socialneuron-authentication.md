---
anonymous_access: false
api_key_in: []
auth_types: []
description: Authentication methods for Social Neuron MCP server
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Socialneuron Authentication
name_suffix: Authentication
oauth_flows: []
overview: Social Neuron declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Social Neuron
provider_slug: socialneuron
scheme_count: 2
schemes:
- evidence: Browser OAuth Flow Standard browser-based OAuth for environments that support redirects.
  flows:
  - authorization_code
  how_to_obtain: Run `npx -y @socialneuron/mcp-server login` which initiates a standard browser OAuth flow.
  name: Browser OAuth Flow
  type: oauth2
- evidence: Generate a key in the Social Neuron dashboard and paste it into the CLI.
  how_to_obtain: Generate your key at https://socialneuron.com/settings/developer and provide it via the CLI with `--paste` or set the `SOCIALNEURON_API_KEY` environment variable.
  name: API Key Paste
  type: apiKey
slug: socialneuron-authentication
source_filename: socialneuron-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.socialneuron.com/guides/authentication
source_yaml: "generated: '2026-10-27'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.socialneuron.com/guides/authentication\nsources:\n- https://docs.socialneuron.com/guides/authentication\n- https://docs.socialneuron.com/guides/mcp-quickstart\n- https://docs.socialneuron.com/docs/getting-started\n- https://socialneuron.com/docs/getting-started\ndescription: Authentication methods for Social Neuron MCP server\nschemes:\n- type: oauth2\n  name: Browser OAuth Flow\n  evidence: Browser OAuth Flow Standard browser-based OAuth for environments that support redirects.\n  flows:\n  - authorization_code\n  how_to_obtain: Run `npx -y @socialneuron/mcp-server login` which initiates a standard browser OAuth flow.\n- type: apiKey\n  name: API Key Paste\n  evidence: Generate a key in the Social Neuron dashboard and paste it into the CLI.\n  how_to_obtain: Generate your key at https://socialneuron.com/settings/developer and provide it via the CLI with `--paste` or\
  \ set the `SOCIALNEURON_API_KEY`\n    environment variable.\ndocs: https://docs.socialneuron.com/guides/authentication\nnote: 1 extracted row(s) were dropped because their quote was not on the page.\n"
source_yaml_url: https://artifacts.apis.io/socialneuron/authentication/socialneuron-authentication.yml
summary_line: 2 schemes
tags:
- Company
- AI
- Content Creation
- Social Media
- Automation
---
