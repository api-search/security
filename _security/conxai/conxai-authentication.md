---
api_key_in:
- header
api_specs:
- filename: conxai-customer-openapi.json
  format: json
  label: Conxai Customer API (SiteLens)
  slug: conxai-customer-api-sitelens
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/conxai/refs/heads/main/openapi/conxai-customer-openapi.json
- filename: conxai-docnostic-openapi.json
  format: json
  label: Conxai Docnostic API
  slug: conxai-docnostic-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/conxai/refs/heads/main/openapi/conxai-docnostic-openapi.json
- filename: conxai-firestop-openapi.json
  format: json
  label: Conxai Firestop API
  slug: conxai-firestop-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/conxai/refs/heads/main/openapi/conxai-firestop-openapi.json
- filename: conxai-production-tracking-openapi.json
  format: json
  label: Conxai Production Tracking API
  slug: conxai-production-tracking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/conxai/refs/heads/main/openapi/conxai-production-tracking-openapi.json
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Conxai Authentication
name_suffix: Authentication
oauth_flows: []
overview: Conxai secures its APIs with apiKey across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Conxai
provider_slug: conxai
scheme_count: 3
schemes:
- description: Provide the given API key
  in: header
  name: ApiKeyAuth
  parameter: X-Api-Key
  sources:
  - openapi/conxai-customer-openapi.json
  - openapi/conxai-docnostic-openapi.json
  - openapi/conxai-firestop-openapi.json
  type: apiKey
- description: Provide the JWT token in the Authorization header prefixed with "Bearer"
  in: header
  name: BearerAuth
  parameter: Authorization
  sources:
  - openapi/conxai-docnostic-openapi.json
  type: apiKey
- in: header
  name: ApiKeyAuth
  parameter: X-API-Key
  sources:
  - openapi/conxai-production-tracking-openapi.json
  type: apiKey
slug: conxai-authentication
source_filename: conxai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: derived\nsource: openapi/conxai-customer-openapi.json, openapi/conxai-docnostic-openapi.json, openapi/conxai-firestop-openapi.json,\n  openapi/conxai-production-tracking-openapi.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-Api-Key\n  description: Provide the given API key\n  sources:\n  - openapi/conxai-customer-openapi.json\n  - openapi/conxai-docnostic-openapi.json\n  - openapi/conxai-firestop-openapi.json\n- name: BearerAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: Provide the JWT token in the Authorization header prefixed with \"Bearer\"\n  sources:\n  - openapi/conxai-docnostic-openapi.json\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  sources:\n  - openapi/conxai-production-tracking-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/conxai/refs/heads/main/authentication/conxai-authentication.yml
summary_line: apiKey · 3 schemes
tags:
- Company
- Construction
- AEC
- Artificial Intelligence
- Document Processing
- Computer Vision
- Agentic AI
- Machine Learning
---
