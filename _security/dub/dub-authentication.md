---
api_key_in: []
api_specs:
- filename: dub-analytics-api-openapi.yml
  format: yaml
  label: Dub Analytics API
  slug: dub-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dub/refs/heads/main/openapi/dub-analytics-api-openapi.yml
- filename: dub-bounties-api-openapi.yml
  format: yaml
  label: Dub Bounties API
  slug: dub-bounties-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dub/refs/heads/main/openapi/dub-bounties-api-openapi.yml
- filename: dub-commissions-api-openapi.yml
  format: yaml
  label: Dub Commissions API
  slug: dub-commissions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dub/refs/heads/main/openapi/dub-commissions-api-openapi.yml
- filename: dub-customers-api-openapi.yml
  format: yaml
  label: Dub Customers API
  slug: dub-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dub/refs/heads/main/openapi/dub-customers-api-openapi.yml
- filename: dub-domains-api-openapi.yml
  format: yaml
  label: Dub Domains API
  slug: dub-domains-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dub/refs/heads/main/openapi/dub-domains-api-openapi.yml
- filename: dub-embed-tokens-api-openapi.yml
  format: yaml
  label: Dub Embed Tokens API
  slug: dub-embed-tokens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dub/refs/heads/main/openapi/dub-embed-tokens-api-openapi.yml
- filename: dub-events-api-openapi.yml
  format: yaml
  label: Dub Events API
  slug: dub-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dub/refs/heads/main/openapi/dub-events-api-openapi.yml
- filename: dub-folders-api-openapi.yml
  format: yaml
  label: Dub Folders API
  slug: dub-folders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dub/refs/heads/main/openapi/dub-folders-api-openapi.yml
- filename: dub-links-api-openapi.yml
  format: yaml
  label: Dub Links API
  slug: dub-links-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dub/refs/heads/main/openapi/dub-links-api-openapi.yml
- filename: dub-partner-applications-api-openapi.yml
  format: yaml
  label: Dub Partner Applications API
  slug: dub-partner-applications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dub/refs/heads/main/openapi/dub-partner-applications-api-openapi.yml
- filename: dub-partners-api-openapi.yml
  format: yaml
  label: Dub Partners API
  slug: dub-partners-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dub/refs/heads/main/openapi/dub-partners-api-openapi.yml
- filename: dub-payouts-api-openapi.yml
  format: yaml
  label: Dub Payouts API
  slug: dub-payouts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dub/refs/heads/main/openapi/dub-payouts-api-openapi.yml
- filename: dub-qr-codes-api-openapi.yml
  format: yaml
  label: Dub QR Codes API
  slug: dub-qr-codes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dub/refs/heads/main/openapi/dub-qr-codes-api-openapi.yml
- filename: dub-tags-api-openapi.yml
  format: yaml
  label: Dub Tags API
  slug: dub-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dub/refs/heads/main/openapi/dub-tags-api-openapi.yml
- filename: dub-track-api-openapi.yml
  format: yaml
  label: Dub Track API
  slug: dub-track-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dub/refs/heads/main/openapi/dub-track-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Dub Authentication
name_suffix: Authentication
oauth_flows: []
overview: Dub secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Dub
provider_slug: dub
scheme_count: 1
schemes:
- description: Default authentication mechanism
  name: token
  scheme: bearer
  sources:
  - openapi/dub-openapi.yml
  type: http
slug: dub-authentication
source_filename: dub-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/dub-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: token\n  type: http\n  scheme: bearer\n  description: Default authentication mechanism\n  sources:\n  - openapi/dub-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dub/refs/heads/main/authentication/dub-authentication.yml
summary_line: http · 1 scheme
tags:
- Link Management
- URL Shortener
- Analytics
- Conversion Tracking
- Affiliate Programs
- Open Source
---
