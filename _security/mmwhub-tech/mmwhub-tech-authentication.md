---
anonymous_access: false
api_key_in: []
api_specs:
- filename: mmwhub-tech-openapi-generated.yml
  format: yaml
  label: MMW API
  slug: mmwhub-tech-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mmwhub-tech/openapi/_ae-authored/mmwhub-tech-openapi-generated.yml
auth_types: []
description: Authentication methods for MMW as documented.
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: MMW Authentication
name_suffix: Authentication
oauth_flows: []
overview: MMW declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: MMW
provider_slug: mmwhub-tech
scheme_count: 2
schemes:
- evidence: 'How it is sent | `Authorization: Bearer mmw_…` header, or the `MMW_API_KEY` variable for mmw-agent. Never in a URL'
  header: Authorization
  how_to_obtain: Create or reveal a personal or organization key in the account under "API Token & Access"; the secret is shown once.
  location: header
  name: MMW API Key
  type: http-bearer
- evidence: 'Web assistants cannot run the local agent and do not keep your key in a config file. They connect to MMW over OAuth: you approve access once on an MMW page, and the assistant receives **its own token valid for 30 days**.'
  how_to_obtain: Add a connector in the assistant (Claude.ai or ChatGPT) with URL `https://mcp.mmwhub.tech/mcp`, then on the MMW consent page paste your API key or sign in with email/password and approve access. The assistant receives a 30‑day token.
  name: Claude.ai / ChatGPT OAuth
  type: oauth2
slug: mmwhub-tech-authentication
source_filename: mmwhub-tech-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.mmwhub.tech/account/api-keys-and-oauth.md
source_yaml: "generated: '2026-11-18'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.mmwhub.tech/account/api-keys-and-oauth.md\nsources:\n- https://docs.mmwhub.tech/account/api-keys-and-oauth.md\n- https://docs.mmwhub.tech/start/quickstart.md\ndescription: Authentication methods for MMW as documented.\nschemes:\n- type: http-bearer\n  name: MMW API Key\n  evidence: 'How it is sent | `Authorization: Bearer mmw_…` header, or the `MMW_API_KEY` variable for mmw-agent. Never in a URL'\n  location: header\n  header: Authorization\n  how_to_obtain: Create or reveal a personal or organization key in the account under \"API Token & Access\"; the secret is shown once.\n- type: oauth2\n  name: Claude.ai / ChatGPT OAuth\n  evidence: 'Web assistants cannot run the local agent and do not keep your key in a config file. They connect to MMW over OAuth: you approve\n    access once on an MMW page, and the assistant receives **its own token valid for 30 days**.'\n  how_to_obtain:\
  \ Add a connector in the assistant (Claude.ai or ChatGPT) with URL `https://mcp.mmwhub.tech/mcp`, then on the MMW consent page\n    paste your API key or sign in with email/password and approve access. The assistant receives a 30‑day token.\ndocs: https://docs.mmwhub.tech/account/api-keys-and-oauth.md\n"
source_yaml_url: https://artifacts.apis.io/mmwhub-tech/authentication/mmwhub-tech-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Artificial Intelligence
- Memory
- Collaboration
- Software-as-a-Service
---
