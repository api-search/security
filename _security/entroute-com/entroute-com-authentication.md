---
anonymous_access: false
api_key_in: []
api_specs:
- filename: entroute-com-openapi-generated.yml
  format: yaml
  label: EntRoute API
  slug: entroute-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/entroute-com/openapi/_ae-authored/entroute-com-openapi-generated.yml
auth_types: []
description: Authentication methods described on EntRoute pages
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: EntRoute Authentication
name_suffix: Authentication
oauth_flows: []
overview: EntRoute declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: EntRoute
provider_slug: entroute-com
scheme_count: 2
schemes:
- evidence: The agent’s only credential is a wallet private key, and it spends from that wallet for every call.
  name: wallet private key
  type: other
- evidence: Rate Limits Anonymous access is rate‑limited. Get higher limits with an API token.
  name: API token
  type: other
slug: entroute-com-authentication
source_filename: entroute-com-authentication.yml
source_heading: Authentication Profile
source_url: https://entroute.com/blog/i-gave-claude-code-five-dollars-and-asked-it-to-research-a-token
source_yaml: "generated: '2026-11-06'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://entroute.com/blog/i-gave-claude-code-five-dollars-and-asked-it-to-research-a-token\nsources:\n- https://entroute.com/blog/i-gave-claude-code-five-dollars-and-asked-it-to-research-a-token\n- https://entroute.com/docs/quickstart\ndescription: Authentication methods described on EntRoute pages\nschemes:\n- type: other\n  name: wallet private key\n  evidence: The agent’s only credential is a wallet private key, and it spends from that wallet for every call.\n- type: other\n  name: API token\n  evidence: Rate Limits Anonymous access is rate‑limited. Get higher limits with an API token.\ndocs: https://entroute.com/blog/i-gave-claude-code-five-dollars-and-asked-it-to-research-a-token\n"
source_yaml_url: https://artifacts.apis.io/entroute-com/authentication/entroute-com-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Discovery
- Artificial Intelligence
- Payments
---
