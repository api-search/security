---
api_key_in:
- header
api_specs:
- filename: wappalyzer-metadata-api-openapi.yml
  format: yaml
  label: Wappalyzer Metadata API
  slug: wappalyzer-metadata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wappalyzer/refs/heads/main/openapi/wappalyzer-metadata-api-openapi.yml
- filename: wappalyzer-basics-api-openapi.yml
  format: yaml
  label: Wappalyzer Basics API
  slug: wappalyzer-basics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wappalyzer/refs/heads/main/openapi/wappalyzer-basics-api-openapi.yml
- filename: wappalyzer-lists-api-openapi.yml
  format: yaml
  label: Wappalyzer Lists API
  slug: wappalyzer-lists-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wappalyzer/refs/heads/main/openapi/wappalyzer-lists-api-openapi.yml
- filename: wappalyzer-lookup-api-openapi.yml
  format: yaml
  label: Wappalyzer Lookup API
  slug: wappalyzer-lookup-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wappalyzer/refs/heads/main/openapi/wappalyzer-lookup-api-openapi.yml
- filename: wappalyzer-subdomains-api-openapi.yml
  format: yaml
  label: Wappalyzer Subdomains API
  slug: wappalyzer-subdomains-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wappalyzer/refs/heads/main/openapi/wappalyzer-subdomains-api-openapi.yml
- filename: wappalyzer-verify-api-openapi.yml
  format: yaml
  label: Wappalyzer Verify API
  slug: wappalyzer-verify-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wappalyzer/refs/heads/main/openapi/wappalyzer-verify-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Wappalyzer Authentication
name_suffix: Authentication
oauth_flows: []
overview: Wappalyzer secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Wappalyzer
provider_slug: wappalyzer
scheme_count: 1
schemes:
- in: header
  name: ApiKeyAuth
  parameter: x-api-key
  sources:
  - openapi/wappalyzer-basics-api-openapi.yml
  - openapi/wappalyzer-lists-api-openapi.yml
  - openapi/wappalyzer-lookup-api-openapi.yml
  - openapi/wappalyzer-subdomains-api-openapi.yml
  - openapi/wappalyzer-verify-api-openapi.yml
  type: apiKey
slug: wappalyzer-authentication
source_filename: wappalyzer-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-14'\nmethod: derived\nsource: openapi/wappalyzer-basics-api-openapi.yml, openapi/wappalyzer-lists-api-openapi.yml,\n  openapi/wappalyzer-lookup-api-openapi.yml, openapi/wappalyzer-subdomains-api-openapi.yml,\n  openapi/wappalyzer-verify-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  sources:\n  - openapi/wappalyzer-basics-api-openapi.yml\n  - openapi/wappalyzer-lists-api-openapi.yml\n  - openapi/wappalyzer-lookup-api-openapi.yml\n  - openapi/wappalyzer-subdomains-api-openapi.yml\n  - openapi/wappalyzer-verify-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wappalyzer/refs/heads/main/authentication/wappalyzer-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Technology Detection
- Technographics
- Website Analysis
- CMS Detection
- Framework Detection
- Lead Enrichment
- Sales Intelligence
- Subdomain Discovery
- Email Verification
- Market Research
---
