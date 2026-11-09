---
anonymous_access: false
api_key_in: []
api_specs:
- filename: budgeyapp-com-openapi-generated.yml
  format: yaml
  label: Budgey API
  slug: budgeyapp-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/budgeyapp-com/openapi/_ae-authored/budgeyapp-com-openapi-generated.yml
auth_types: []
description: Authentication methods for Budgey
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Budgeyapp Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: Budgey declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Budgey
provider_slug: budgeyapp-com
scheme_count: 2
schemes:
- evidence: A browser window opens on Budgey. Sign in, then tap Allow access . Your agent receives tokens and can call budgeting tools as you.
  how_to_obtain: Browser sign‑in and allow access; tokens are received after OAuth flow.
  name: OAuth
  type: oauth2
- evidence: '--header "Authorization: Bearer budgey_sk_YOUR_KEY"'
  header: Authorization
  how_to_obtain: 'Create a budgey_sk_… key at Settings → AI agents and send it in the Authorization: Bearer header.'
  location: header
  name: API key
  type: apiKey
slug: budgeyapp-com-authentication
source_filename: budgeyapp-com-authentication.yml
source_heading: Authentication Profile
source_url: https://www.budgeyapp.com/developers
source_yaml: "generated: '2026-11-03'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://www.budgeyapp.com/developers\nsources:\n- https://www.budgeyapp.com/developers\ndescription: Authentication methods for Budgey\nschemes:\n- type: oauth2\n  name: OAuth\n  evidence: A browser window opens on Budgey. Sign in, then tap Allow access . Your agent receives tokens and can call budgeting tools as you.\n  how_to_obtain: Browser sign‑in and allow access; tokens are received after OAuth flow.\n- type: apiKey\n  name: API key\n  evidence: '--header \"Authorization: Bearer budgey_sk_YOUR_KEY\"'\n  location: header\n  header: Authorization\n  how_to_obtain: 'Create a budgey_sk_… key at Settings → AI agents and send it in the Authorization: Bearer header.'\ndocs: https://www.budgeyapp.com/developers\n"
source_yaml_url: https://artifacts.apis.io/budgeyapp-com/authentication/budgeyapp-com-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Budgeting
- Finance
- Personal Finance
- AI Agents
---
