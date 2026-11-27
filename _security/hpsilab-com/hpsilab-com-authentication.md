---
anonymous_access: false
api_key_in: []
api_specs:
- filename: hpsilab-com-openapi-generated.yml
  format: yaml
  label: HPSILab API
  slug: hpsilab-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hpsilab-com/openapi/_ae-authored/hpsilab-com-openapi-generated.yml
auth_types: []
description: Authentication methods published on HPSILab pages
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: HPSILab Authentication
name_suffix: Authentication
oauth_flows: []
overview: HPSILab declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: HPSILab
provider_slug: hpsilab-com
scheme_count: 2
schemes:
- evidence: 'REST API Authenticate with your API key. Copy curl https://hpsilab.com/api/analyze_stock/NVDA \ -H "Authorization: Bearer hpsi_your_key"'
  header: Authorization
  how_to_obtain: API key issued automatically after sign‑in; no manual creation required
  location: header
  name: API Key
  type: http-bearer
- authorize_url: https://hpsilab.com/oauth/authorize
  evidence: 'OAuth 2.1 with Dynamic Client Registration (DCR). An HPSILab account is required: your MCP client opens sign-in and is issued its API key automatically, so you never create one by hand.'
  how_to_obtain: Dynamic client registration; client opens sign‑in to obtain credentials
  name: OAuth 2.1
  token_url: https://hpsilab.com/oauth/token
  type: oauth2
slug: hpsilab-com-authentication
source_filename: hpsilab-com-authentication.yml
source_heading: Authentication Profile
source_url: https://hpsilab.com/.well-known/oauth-authorization-server
source_yaml: "generated: '2026-11-11'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://hpsilab.com/.well-known/oauth-authorization-server\nsources:\n- https://hpsilab.com/.well-known/oauth-authorization-server\n- https://hpsilab.com/login?next=%2Fsettings\n- https://hpsilab.com/developer/v2\ndescription: Authentication methods published on HPSILab pages\nschemes:\n- type: http-bearer\n  name: API Key\n  evidence: 'REST API Authenticate with your API key. Copy curl https://hpsilab.com/api/analyze_stock/NVDA \\ -H \"Authorization: Bearer hpsi_your_key\"'\n  location: header\n  header: Authorization\n  how_to_obtain: API key issued automatically after sign‑in; no manual creation required\n- type: oauth2\n  name: OAuth 2.1\n  evidence: 'OAuth 2.1 with Dynamic Client Registration (DCR). An HPSILab account is required: your MCP client opens sign-in and is issued its\n    API key automatically, so you never create one by hand.'\n  token_url: https://hpsilab.com/oauth/token\n\
  \  authorize_url: https://hpsilab.com/oauth/authorize\n  how_to_obtain: Dynamic client registration; client opens sign‑in to obtain credentials\ndocs: https://hpsilab.com/.well-known/oauth-authorization-server\n"
source_yaml_url: https://artifacts.apis.io/hpsilab-com/authentication/hpsilab-com-authentication.yml
summary_line: 2 schemes
tags:
- Finance
- Quant
- Artificial Intelligence
- Stocks
- Options
---
