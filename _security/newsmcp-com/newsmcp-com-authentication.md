---
anonymous_access: false
api_key_in: []
api_specs:
- filename: newsmcp-com-health-api-openapi.yml
  format: yaml
  label: NewsMCP Health API
  slug: newsmcp-com-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/newsmcp-com/openapi/newsmcp-com-health-api-openapi.yml
- filename: newsmcp-com-limits-api-openapi.yml
  format: yaml
  label: NewsMCP Limits API
  slug: newsmcp-com-limits-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/newsmcp-com/openapi/newsmcp-com-limits-api-openapi.yml
- filename: newsmcp-com-news-api-openapi.yml
  format: yaml
  label: NewsMCP News API
  slug: newsmcp-com-news-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/newsmcp-com/openapi/newsmcp-com-news-api-openapi.yml
auth_types: []
description: Authentication methods for NewsMCP are described on the onboarding page.
kind: authentication
layout: security
mechanism_count: 4
method: searched
name: NewsMCP Authentication
name_suffix: Authentication
oauth_flows: []
overview: NewsMCP declares 4 security scheme(s) across its OpenAPI definitions.
provider_name: NewsMCP
provider_slug: newsmcp-com
scheme_count: 4
schemes:
- evidence: Sign in (OAuth) | https://mcp.newsmcp.com/mcp?login | Yes — a NewsMCP account; the client opens sign-in, no key to copy
  how_to_obtain: The client opens the URL https://mcp.newsmcp.com/mcp?login, signs in with a NewsMCP account, and receives an API key automatically.
  name: Sign in (OAuth)
  type: oauth2
- evidence: API key | https://mcp.newsmcp.com/mcp + key (header or `?apiKey=`) | Yes, to create the key
  header: x-api-key
  how_to_obtain: Create a key in the NewsMCP platform at https://platform.newsmcp.com/auth and paste it into the x‑api‑key header or add it as the query parameter apiKey.
  location: header
  name: API key
  type: apiKey
- evidence: API key | https://mcp.newsmcp.com/mcp + key (header or `?apiKey=`) | Yes, to create the key
  header: apiKey
  how_to_obtain: Create a key in the NewsMCP platform at https://platform.newsmcp.com/auth and append it as the apiKey query parameter.
  location: query
  name: API key (query)
  type: apiKey
- evidence: Keyless | https://mcp.newsmcp.com/mcp | No
  how_to_obtain: No credentials required; use the endpoint without any authentication headers or query parameters.
  name: Keyless (no authentication)
  type: other
slug: newsmcp-com-authentication
source_filename: newsmcp-com-authentication.yml
source_heading: Authentication Profile
source_url: https://newsmcp.com/agent-onboarding/SKILL.md
source_yaml: "generated: '2026-11-19'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://newsmcp.com/agent-onboarding/SKILL.md\nsources:\n- https://newsmcp.com/agent-onboarding/SKILL.md\ndescription: Authentication methods for NewsMCP are described on the onboarding page.\nschemes:\n- type: oauth2\n  name: Sign in (OAuth)\n  evidence: Sign in (OAuth) | https://mcp.newsmcp.com/mcp?login | Yes — a NewsMCP account; the client opens sign-in, no key to copy\n  how_to_obtain: The client opens the URL https://mcp.newsmcp.com/mcp?login, signs in with a NewsMCP account, and receives an API key automatically.\n- type: apiKey\n  name: API key\n  evidence: API key | https://mcp.newsmcp.com/mcp + key (header or `?apiKey=`) | Yes, to create the key\n  location: header\n  header: x-api-key\n  how_to_obtain: Create a key in the NewsMCP platform at https://platform.newsmcp.com/auth and paste it into the x‑api‑key header or add it as\n    the query parameter apiKey.\n- type:\
  \ apiKey\n  name: API key (query)\n  evidence: API key | https://mcp.newsmcp.com/mcp + key (header or `?apiKey=`) | Yes, to create the key\n  location: query\n  header: apiKey\n  how_to_obtain: Create a key in the NewsMCP platform at https://platform.newsmcp.com/auth and append it as the apiKey query parameter.\n- type: other\n  name: Keyless (no authentication)\n  evidence: Keyless | https://mcp.newsmcp.com/mcp | No\n  how_to_obtain: No credentials required; use the endpoint without any authentication headers or query parameters.\ndocs: https://newsmcp.com/agent-onboarding/SKILL.md\n"
source_yaml_url: https://artifacts.apis.io/newsmcp-com/authentication/newsmcp-com-authentication.yml
summary_line: 4 schemes
tags:
- News
- Artificial Intelligence
- News API
- MCP
- Aggregation
---
