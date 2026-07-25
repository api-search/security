---
api_key_in:
- header
api_specs:
- filename: trustradius-categories-api-openapi.yml
  format: yaml
  label: TrustRadius Categories API
  slug: trustradius-categories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trustradius/refs/heads/main/openapi/trustradius-categories-api-openapi.yml
- filename: trustradius-companies-api-openapi.yml
  format: yaml
  label: TrustRadius Companies API
  slug: trustradius-companies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trustradius/refs/heads/main/openapi/trustradius-companies-api-openapi.yml
- filename: trustradius-products-api-openapi.yml
  format: yaml
  label: TrustRadius Products API
  slug: trustradius-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trustradius/refs/heads/main/openapi/trustradius-products-api-openapi.yml
- filename: trustradius-reviews-api-openapi.yml
  format: yaml
  label: TrustRadius Reviews API
  slug: trustradius-reviews-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trustradius/refs/heads/main/openapi/trustradius-reviews-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Trustradius Authentication
name_suffix: Authentication
oauth_flows: []
overview: TrustRadius secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: TrustRadius
provider_slug: trustradius
scheme_count: 1
schemes:
- description: TrustRadius API key obtained from Vendor Portal > Integrations
  in: header
  name: ApiKey
  parameter: X-API-Key
  sources:
  - openapi/trustradius-public-openapi.yml
  - openapi/trustradius-reviews-openapi.yml
  type: apiKey
slug: trustradius-authentication
source_filename: trustradius-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/trustradius-public-openapi.yml, openapi/trustradius-reviews-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKey\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  description: TrustRadius API key obtained from Vendor Portal > Integrations\n  sources:\n  - openapi/trustradius-public-openapi.yml\n  - openapi/trustradius-reviews-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/trustradius/refs/heads/main/authentication/trustradius-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- B2B Software Reviews
- Buyer Intelligence
- Intent Data
- Software Reviews
- Reviews
- Product Reviews
- Categories
---
