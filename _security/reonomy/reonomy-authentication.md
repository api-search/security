---
api_key_in: []
api_specs:
- filename: reonomy-openapi.yml
  format: yaml
  label: Reonomy Property Search API
  slug: property-search
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reonomy/refs/heads/main/openapi/reonomy-openapi.yml
- filename: reonomy-openapi.yml
  format: yaml
  label: Reonomy Property Detail API
  slug: property-detail
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reonomy/refs/heads/main/openapi/reonomy-openapi.yml
- filename: reonomy-openapi.yml
  format: yaml
  label: Reonomy Ownership API
  slug: ownership
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reonomy/refs/heads/main/openapi/reonomy-openapi.yml
- filename: reonomy-openapi.yml
  format: yaml
  label: Reonomy Sales & Debt API
  slug: sales-debt
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reonomy/refs/heads/main/openapi/reonomy-openapi.yml
- filename: reonomy-openapi.yml
  format: yaml
  label: Reonomy Tenants API
  slug: tenants
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reonomy/refs/heads/main/openapi/reonomy-openapi.yml
- filename: reonomy-openapi.yml
  format: yaml
  label: Reonomy Contacts API
  slug: contacts
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reonomy/refs/heads/main/openapi/reonomy-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Reonomy Authentication
name_suffix: Authentication
oauth_flows: []
overview: Reonomy secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Reonomy
provider_slug: reonomy
scheme_count: 1
schemes:
- description: HTTP Basic Authentication. The Authorization header carries a base64-encoded access_key:secret_key access token issued by Reonomy.
  name: basicAuth
  scheme: basic
  sources:
  - openapi/reonomy-openapi.yml
  type: http
slug: reonomy-authentication
source_filename: reonomy-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/reonomy-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: HTTP Basic Authentication. The Authorization header carries a base64-encoded\n    access_key:secret_key access token issued by Reonomy.\n  sources:\n  - openapi/reonomy-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/reonomy/refs/heads/main/authentication/reonomy-authentication.yml
summary_line: http · 1 scheme
tags:
- Commercial Real Estate
- Property Data
- Property Intelligence
- Ownership
- Skip Trace
---
