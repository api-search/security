---
anonymous_access: false
api_key_in: []
api_specs:
- filename: quiver-quantitative-beta-api-openapi.yml
  format: yaml
  label: Quiver Quantitative Beta API
  slug: quiver-quantitative-beta-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quiver-quantitative/refs/heads/main/openapi/quiver-quantitative-beta-api-openapi.yml
- filename: quiver-quantitative-tier-1-api-openapi.yml
  format: yaml
  label: Quiver Quantitative Tier 1 API
  slug: quiver-quantitative-tier-1-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quiver-quantitative/refs/heads/main/openapi/quiver-quantitative-tier-1-api-openapi.yml
- filename: quiver-quantitative-tier-2-api-openapi.yml
  format: yaml
  label: Quiver Quantitative Tier 2 API
  slug: quiver-quantitative-tier-2-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quiver-quantitative/refs/heads/main/openapi/quiver-quantitative-tier-2-api-openapi.yml
- filename: quiver-quantitative-tier-new-constructs-ratings-api-openapi.yml
  format: yaml
  label: Quiver Quantitative Tier New Constructs Ratings API
  slug: quiver-quantitative-tier-new-constructs-ratings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quiver-quantitative/refs/heads/main/openapi/quiver-quantitative-tier-new-constructs-ratings-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Quiver Quantitative Authentication
name_suffix: Authentication
oauth_flows: []
overview: Quiver Quantitative secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Quiver Quantitative
provider_slug: quiver-quantitative
scheme_count: 1
schemes:
- name: WebPlatformTokenAuth
  scheme: bearer
  sources:
  - openapi/quiver-quantitative-openapi.json
  type: http
slug: quiver-quantitative-authentication
source_filename: quiver-quantitative-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-21'\nmethod: derived\nsource: openapi/quiver-quantitative-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: WebPlatformTokenAuth\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/quiver-quantitative-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/quiver-quantitative/refs/heads/main/authentication/quiver-quantitative-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Data
- Finance
- Politics
---
