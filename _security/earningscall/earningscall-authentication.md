---
anonymous_access: false
api_key_in: []
api_specs:
- filename: earningscall-openapi-generated.yml
  format: yaml
  label: EarningsCall API
  slug: earningscall-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/earningscall/refs/heads/main/openapi/_ae-authored/earningscall-openapi-generated.yml
auth_types: []
description: Every request to the EarningsCall API must include an API key. You can send it as a query parameter or as the x-api-key header.
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Earningscall Authentication
name_suffix: Authentication
oauth_flows: []
overview: EarningsCall declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: EarningsCall
provider_slug: earningscall
scheme_count: 2
schemes:
- evidence: Every request to the EarningsCall API must include an API key. You can send it as a query parameter or as the x-api-key header.
  how_to_obtain: Your account dashboard has a single API key tied to your subscription plan.
  location: query
  name: API Key (query)
  type: apiKey
- evidence: Every request to the EarningsCall API must include an API key. You can send it as a query parameter or as the x-api-key header.
  header: x-api-key
  how_to_obtain: Your account dashboard has a single API key tied to your subscription plan.
  location: header
  name: API Key (header)
  type: apiKey
slug: earningscall-authentication
source_filename: earningscall-authentication.yml
source_heading: Authentication Profile
source_url: https://earningscall.biz/docs/authentication
source_yaml: "generated: '2026-10-16'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://earningscall.biz/docs/authentication\nsources:\n- https://earningscall.biz/docs/authentication\ndescription: Every request to the EarningsCall API must include an API key. You can send it as a query parameter or as the x-api-key header.\nschemes:\n- type: apiKey\n  name: API Key (query)\n  evidence: Every request to the EarningsCall API must include an API key. You can send it as a query parameter or as the x-api-key header.\n  location: query\n  how_to_obtain: Your account dashboard has a single API key tied to your subscription plan.\n- type: apiKey\n  name: API Key (header)\n  evidence: Every request to the EarningsCall API must include an API key. You can send it as a query parameter or as the x-api-key header.\n  location: header\n  header: x-api-key\n  how_to_obtain: Your account dashboard has a single API key tied to your subscription plan.\nnote: The reserved demo\
  \ key \"demo\" can be used without sign‑up.\ndocs: https://earningscall.biz/docs/authentication\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/earningscall/refs/heads/main/authentication/earningscall-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Finance
- Data
- API
- Earnings
---
