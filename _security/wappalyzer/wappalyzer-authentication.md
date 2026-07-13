---
api_key_in:
- header
api_specs:
- filename: v2-public.yaml
  format: yaml
  label: Wappalyzer Lookup API
  slug: wappalyzer-lookup-api
  spec_type: OpenAPI
  url: https://www.wappalyzer.com/openapi/v2-public.yaml
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
  - openapi/wappalyzer-lookup-openapi.yml
  type: apiKey
slug: wappalyzer-authentication
source_filename: wappalyzer-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/wappalyzer-lookup-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  sources:\n  - openapi/wappalyzer-lookup-openapi.yml\n"
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
---
