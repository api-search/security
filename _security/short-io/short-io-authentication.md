---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: short-io-audit-api-openapi.yml
  format: yaml
  label: Short.io Audit API
  slug: short-io-audit-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/short-io/openapi/short-io-audit-api-openapi.yml
- filename: short-io-domain-dns-api-openapi.yml
  format: yaml
  label: Short.io Domain DNS API
  slug: short-io-domain-dns-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/short-io/openapi/short-io-domain-dns-api-openapi.yml
- filename: short-io-domains-api-openapi.yml
  format: yaml
  label: Short.io Domains API
  slug: short-io-domains-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/short-io/openapi/short-io-domains-api-openapi.yml
- filename: short-io-link-bundles-api-openapi.yml
  format: yaml
  label: Short.io Link Bundles API
  slug: short-io-link-bundles-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/short-io/openapi/short-io-link-bundles-api-openapi.yml
- filename: short-io-link-duplication-api-openapi.yml
  format: yaml
  label: Short.io Link Duplication API
  slug: short-io-link-duplication-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/short-io/openapi/short-io-link-duplication-api-openapi.yml
- filename: short-io-link-management-api-openapi.yml
  format: yaml
  label: Short.io Link Management API
  slug: short-io-link-management-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/short-io/openapi/short-io-link-management-api-openapi.yml
- filename: short-io-link-queries-api-openapi.yml
  format: yaml
  label: Short.io Link queries API
  slug: short-io-link-queries-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/short-io/openapi/short-io-link-queries-api-openapi.yml
- filename: short-io-link-targeting-api-openapi.yml
  format: yaml
  label: Short.io Link Targeting API
  slug: short-io-link-targeting-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/short-io/openapi/short-io-link-targeting-api-openapi.yml
- filename: short-io-organizations-api-openapi.yml
  format: yaml
  label: Short.io Organizations API
  slug: short-io-organizations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/short-io/openapi/short-io-organizations-api-openapi.yml
- filename: short-io-posts-api-openapi.yml
  format: yaml
  label: Short.io Posts API
  slug: short-io-posts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/short-io/openapi/short-io-posts-api-openapi.yml
- filename: short-io-qr-codes-api-openapi.yml
  format: yaml
  label: Short.io QR Codes API
  slug: short-io-qr-codes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/short-io/openapi/short-io-qr-codes-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Short Io Authentication
name_suffix: Authentication
oauth_flows: []
overview: Short.io secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Short.io
provider_slug: short-io
scheme_count: 1
schemes:
- in: header
  name: apiKey
  parameter: Authorization
  sources:
  - openapi/short-io-openapi.json
  type: apiKey
slug: short-io-authentication
source_filename: short-io-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-27'\nmethod: derived\nsource: openapi/short-io-openapi.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: Authorization\n  sources:\n  - openapi/short-io-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/short-io/authentication/short-io-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- URL-shortening
- Analytics
- QR-codes
- Enterprise
- Integrations
---
