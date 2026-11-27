---
anonymous_access: false
api_key_in: []
api_specs:
- filename: launchdistro-com-openapi-generated.yml
  format: yaml
  label: LaunchDistro API
  slug: launchdistro-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/launchdistro-com/openapi/_ae-authored/launchdistro-com-openapi-generated.yml
auth_types: []
description: Authentication methods for LaunchDistro MCP
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: LaunchDistro Authentication
name_suffix: Authentication
oauth_flows: []
overview: LaunchDistro declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: LaunchDistro
provider_slug: launchdistro-com
scheme_count: 2
schemes:
- evidence: You add its address and a token made for your app, and your agent gets the tools.
  header: Authorization
  how_to_obtain: Create a key for the app in the dashboard; the token (ld_agent_...) is shown once.
  location: header
  name: LaunchDistro token
  type: http-bearer
- evidence: 'You need no token here: the connector signs in to your LaunchDistro account with OAuth, and you approve it on a consent screen.'
  how_to_obtain: The connector initiates an OAuth flow; the user approves on a consent screen.
  name: Claude Desktop connector OAuth
  type: oauth2
slug: launchdistro-com-authentication
source_filename: launchdistro-com-authentication.yml
source_heading: Authentication Profile
source_url: https://launchdistro.com/docs/setup
source_yaml: "generated: '2026-11-15'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://launchdistro.com/docs/setup\nsources:\n- https://launchdistro.com/docs/setup\ndescription: Authentication methods for LaunchDistro MCP\nschemes:\n- type: http-bearer\n  name: LaunchDistro token\n  evidence: You add its address and a token made for your app, and your agent gets the tools.\n  location: header\n  header: Authorization\n  how_to_obtain: Create a key for the app in the dashboard; the token (ld_agent_...) is shown once.\n- type: oauth2\n  name: Claude Desktop connector OAuth\n  evidence: 'You need no token here: the connector signs in to your LaunchDistro account with OAuth, and you approve it on a consent screen.'\n  how_to_obtain: The connector initiates an OAuth flow; the user approves on a consent screen.\ndocs: https://launchdistro.com/docs/setup\n"
source_yaml_url: https://artifacts.apis.io/launchdistro-com/authentication/launchdistro-com-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Artificial Intelligence
- Startups
- SEO
- Automation
---
