---
api_key_in: []
auth_types: []
description: API key passed in the Authorization header. A free key is issued instantly, with no card and no sales call.
kind: authentication
layout: security
method: searched
name: Fundz Authentication
name_suffix: Authentication
oauth_flows: []
overview: Fundz declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Fundz
provider_slug: fundz
scheme_count: 1
schemes:
- example: 'curl -H "Authorization: YOUR_API_KEY" https://api.fundz.net/companies/onelayer'
  id: ApiKey
  in: header
  name: Authorization
  type: apiKey
slug: fundz-authentication
source_filename: fundz-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-03'\nmethod: searched\nstatus: published\nsource: https://app.fundz.net/knowledge/api-references/companies\ndescription: API key passed in the Authorization header. A free key is issued instantly,\n  with no card and no sales call.\nverified: '2026-08-03'\nschemes:\n- id: ApiKey\n  type: apiKey\n  in: header\n  name: Authorization\n  example: 'curl -H \"Authorization: YOUR_API_KEY\" https://api.fundz.net/companies/onelayer'\ntrial:\n  url: https://fundz.net/api-trial\n  instant: true\n  card_required: false\n  note: Free instant key — the differentiator the founder leads with against Crunchbase,\n    whose Basic API was retired.\nevidence:\n- url: https://fundz.net/api-trial\n  status: 200\n- url: https://app.fundz.net/knowledge/api-references/companies\n  status: 200\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fundz/refs/heads/main/authentication/fundz-authentication.yml
summary_line: 1 scheme
tags:
- Business Intelligence
- Funding
- Private Markets
- Mergers And Acquisitions
- SEC Filings
- Signals
- Sales Intelligence
- MCP
- Agents
---
