---
api_key_in:
- header
api_specs:
- filename: tetrascience-openapi.yml
  format: yaml
  label: Tetra Scientific Data and AI Cloud API
  slug: tetra-data-and-ai-cloud-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tetrascience/refs/heads/main/openapi/tetrascience-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Tetrascience Authentication
name_suffix: Authentication
oauth_flows: []
overview: TetraScience secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: TetraScience
provider_slug: tetrascience
scheme_count: 2
schemes:
- description: JWT Token for authentication
  in: header
  name: token
  parameter: ts-auth-token
  sources:
  - openapi/tetrascience-openapi.json
  - openapi/tetrascience-openapi.yml
  type: apiKey
- description: Your organization slug
  in: header
  name: orgSlug
  parameter: x-org-slug
  sources:
  - openapi/tetrascience-openapi.json
  - openapi/tetrascience-openapi.yml
  type: apiKey
slug: tetrascience-authentication
source_filename: tetrascience-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/tetrascience-openapi.json, openapi/tetrascience-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: token\n  type: apiKey\n  in: header\n  parameter: ts-auth-token\n  description: JWT Token for authentication\n  sources:\n  - openapi/tetrascience-openapi.json\n  - openapi/tetrascience-openapi.yml\n- name: orgSlug\n  type: apiKey\n  in: header\n  parameter: x-org-slug\n  description: Your organization slug\n  sources:\n  - openapi/tetrascience-openapi.json\n  - openapi/tetrascience-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tetrascience/refs/heads/main/authentication/tetrascience-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Scientific Data
- Life Sciences
- Pharma
- Biotech
- Lab Data
- Lab Automation
- Data Platform
- Data Engineering
- AI Platform
- Scientific AI
- FAIR Data
- GxP Compliance
- Chromatography
- Spectroscopy
- Cloud Data Lake
- Pipelines
- Agents
- IDS
---
