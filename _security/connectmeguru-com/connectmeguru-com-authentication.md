---
anonymous_access: false
api_key_in: []
api_specs:
- filename: connectmeguru-com-agentic-api-openapi.yml
  format: yaml
  label: ConnectMeGuru Agentic API
  slug: connectmeguru-com-agentic-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/connectmeguru-com/openapi/connectmeguru-com-agentic-api-openapi.yml
- filename: connectmeguru-com-discount-api-openapi.yml
  format: yaml
  label: ConnectMeGuru Discount API
  slug: connectmeguru-com-discount-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/connectmeguru-com/openapi/connectmeguru-com-discount-api-openapi.yml
- filename: connectmeguru-com-products-api-openapi.yml
  format: yaml
  label: ConnectMeGuru Products API
  slug: connectmeguru-com-products-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/connectmeguru-com/openapi/connectmeguru-com-products-api-openapi.yml
auth_types:
- http
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 3
method: searched
name: ConnectMeGuru Authentication
name_suffix: Authentication
oauth_flows: []
overview: ConnectMeGuru secures its APIs with http and apiKey across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: ConnectMeGuru
provider_slug: connectmeguru-com
scheme_count: 3
schemes:
- api: ConnectMeGuru Autonomous Agentic Commerce API
  bearerFormat: PAT
  description: Machine-to-machine Personal Access Token (PAT) generated via /api/agentic/auth/verify-otp or ConnectMeGuru dashboard profile.
  flow: 'Developer page: "One-time OTP verification issues a permanent Personal Access Token (`cmg_pat_...`)."'
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/connectmeguru-com-agentic-openapi.yml
  - https://www.connectmeguru.com/developers/agentic
  token_prefix: cmg_pat_
  type: http
- api: ConnectMeGuru B2B Wholesale API
  description: Every request to the ConnectMeGuru Wholesale API must be authenticated using your API Key and Secret passed as custom HTTP headers.
  headers:
  - description: Your public API key identifier (starts with cmg_live_... ).
    name: X-B2B-Key
  - description: Your confidential API secret key (starts with cmg_sec_... ). Never expose this in client-side code!
    name: X-B2B-Secret
  in: header
  name: B2BKeyAndSecret
  note: Documented on the partner portal only; no OpenAPI is published for the B2B Wholesale API.
  sources:
  - https://partner.connectmeguru.com/docs
  type: apiKey
- api: ConnectMeGuru Travel eSIM API
  description: The travel-esim OpenAPI (catalog, coupons, discount validation) declares no securitySchemes.
  name: none
  sources:
  - openapi/connectmeguru-com-travel-esim-openapi.yml
slug: connectmeguru-com-authentication
source_filename: connectmeguru-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: searched\nsource:\n- https://partner.connectmeguru.com/docs\n- https://www.connectmeguru.com/developers/agentic\ndocs: https://partner.connectmeguru.com/docs\nsummary:\n  types:\n  - http\n  - apiKey\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: PAT\n  api: ConnectMeGuru Autonomous Agentic Commerce API\n  description: Machine-to-machine Personal Access Token (PAT) generated via /api/agentic/auth/verify-otp\n    or ConnectMeGuru dashboard profile.\n  token_prefix: cmg_pat_\n  flow: 'Developer page: \"One-time OTP verification issues a permanent Personal Access Token (`cmg_pat_...`).\"'\n  sources:\n  - openapi/connectmeguru-com-agentic-openapi.yml\n  - https://www.connectmeguru.com/developers/agentic\n- name: B2BKeyAndSecret\n  type: apiKey\n  in: header\n  api: ConnectMeGuru B2B Wholesale API\n  headers:\n  - name: X-B2B-Key\n    description: Your public API key identifier (starts with cmg_live_... ).\n  - name:\
  \ X-B2B-Secret\n    description: Your confidential API secret key (starts with cmg_sec_... ). Never expose this in client-side code!\n  description: Every request to the ConnectMeGuru Wholesale API must be authenticated using your API Key and\n    Secret passed as custom HTTP headers.\n  note: Documented on the partner portal only; no OpenAPI is published for the B2B Wholesale API.\n  sources:\n  - https://partner.connectmeguru.com/docs\n- name: none\n  api: ConnectMeGuru Travel eSIM API\n  description: The travel-esim OpenAPI (catalog, coupons, discount validation) declares no securitySchemes.\n  sources:\n  - openapi/connectmeguru-com-travel-esim-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/connectmeguru-com/authentication/connectmeguru-com-authentication.yml
summary_line: http/apiKey · 3 schemes
tags:
- Company
- eSIM
- Travel
- Telecommunications
- Mobile Data
- Connectivity
- Wholesale
- MCP
- AI Agents
---
