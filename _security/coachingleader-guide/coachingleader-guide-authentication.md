---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: coachingleader-guide-openapi.yml
  format: yaml
  label: Bicycle Guide Guide Registry API
  slug: guide-registry-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coachingleader-guide/openapi/coachingleader-guide-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Coaching Leader Guide Authentication
name_suffix: Authentication
oauth_flows: []
overview: Coaching Leader Guide secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Coaching Leader Guide
provider_slug: coachingleader-guide
scheme_count: 1
schemes:
- description: 'Authorization: Bearer $BICYCLE_GUIDE_API_SECRET, or the x-bicycle-guide-secret header with the same value. Unset secret ⇒ 503 (fails closed, never open data). Missing/invalid credentials ⇒ 401.'
  in: header
  name: bicycleGuideSecret
  parameter: x-bicycle-guide-secret
  sources:
  - openapi/coachingleader-guide-openapi.yml
  type: apiKey
slug: coachingleader-guide-authentication
source_filename: coachingleader-guide-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: searched\nsource: https://coachingleader.guide/llms.txt\ndocs: https://coachingleader.guide/llms.txt\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: bicycleGuideSecret\n  type: apiKey\n  in: header\n  parameter: x-bicycle-guide-secret\n  description: 'Authorization: Bearer $BICYCLE_GUIDE_API_SECRET, or the x-bicycle-guide-secret\n    header with the same value. Unset secret ⇒ 503 (fails closed, never open data). Missing/invalid\n    credentials ⇒ 401.'\n  sources:\n  - openapi/coachingleader-guide-openapi.yml\nunauthenticated_surfaces:\n- surface: MCP server\n  url: https://coachingleader.guide/mcp\n  statement: \"remote Model Context Protocol access to the guide registry, taxonomy and capability spine — read-only, no auth required.\"\n  source: https://coachingleader.guide/llms.txt\nnote: >-\n  The shared secret is not issued through any documented self-serve flow; the OpenAPI describes it as\n  \"read-only control-plane\
  \ metadata for cooperating repos and agents\". The docs URL the spec cites\n  (https://bicycle.guide/docs) returned HTTP 404 on 2026-11-04.\n"
source_yaml_url: https://artifacts.apis.io/coachingleader-guide/authentication/coachingleader-guide-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Coaching
- Leadership
- Management
- Education
- Books
- MCP
---
