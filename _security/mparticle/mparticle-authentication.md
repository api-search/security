---
api_key_in: []
api_specs:
- filename: mparticle-openapi.yml
  format: yaml
  label: mParticle Events API
  slug: events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mparticle/refs/heads/main/openapi/mparticle-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Mparticle Authentication
name_suffix: Authentication
oauth_flows: []
overview: mParticle secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: mParticle
provider_slug: mparticle
scheme_count: 1
schemes:
- description: HTTP Basic Auth using API key as username and secret as password.
  name: basicAuth
  scheme: basic
  sources:
  - openapi/mparticle-openapi.yml
  type: http
slug: mparticle-authentication
source_filename: mparticle-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/mparticle-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: HTTP Basic Auth using API key as username and secret as password.\n  sources:\n  - openapi/mparticle-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mparticle/refs/heads/main/authentication/mparticle-authentication.yml
summary_line: http · 1 scheme
tags:
- Customer Data Platform
- CDP
- Analytics
- Identity Resolution
- Audience
- Data Pipeline
- Marketing Data
---
