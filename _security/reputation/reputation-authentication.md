---
api_key_in:
- header
api_specs:
- filename: reputation-asset-library-api-openapi.yml
  format: yaml
  label: Reputation Asset Library API
  slug: reputation-asset-library-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reputation/refs/heads/main/openapi/reputation-asset-library-api-openapi.yml
- filename: reputation-authorize-api-openapi.yml
  format: yaml
  label: Reputation Authorize API
  slug: reputation-authorize-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reputation/refs/heads/main/openapi/reputation-authorize-api-openapi.yml
- filename: reputation-categories-api-openapi.yml
  format: yaml
  label: Reputation Categories API
  slug: reputation-categories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reputation/refs/heads/main/openapi/reputation-categories-api-openapi.yml
- filename: reputation-credentials-api-openapi.yml
  format: yaml
  label: Reputation Credentials API
  slug: reputation-credentials-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reputation/refs/heads/main/openapi/reputation-credentials-api-openapi.yml
- filename: reputation-listing-audits-api-openapi.yml
  format: yaml
  label: Reputation Listing Audits API
  slug: reputation-listing-audits-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reputation/refs/heads/main/openapi/reputation-listing-audits-api-openapi.yml
- filename: reputation-locations-api-openapi.yml
  format: yaml
  label: Reputation Locations API
  slug: reputation-locations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reputation/refs/heads/main/openapi/reputation-locations-api-openapi.yml
- filename: reputation-metrics-api-openapi.yml
  format: yaml
  label: Reputation Metrics API
  slug: reputation-metrics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reputation/refs/heads/main/openapi/reputation-metrics-api-openapi.yml
- filename: reputation-reports-api-openapi.yml
  format: yaml
  label: Reputation Reports API
  slug: reputation-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reputation/refs/heads/main/openapi/reputation-reports-api-openapi.yml
- filename: reputation-requests-api-openapi.yml
  format: yaml
  label: Reputation Requests API
  slug: reputation-requests-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reputation/refs/heads/main/openapi/reputation-requests-api-openapi.yml
- filename: reputation-reviews-api-openapi.yml
  format: yaml
  label: Reputation Reviews API
  slug: reputation-reviews-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reputation/refs/heads/main/openapi/reputation-reviews-api-openapi.yml
- filename: reputation-rich-content-api-openapi.yml
  format: yaml
  label: Reputation Rich Content API
  slug: reputation-rich-content-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reputation/refs/heads/main/openapi/reputation-rich-content-api-openapi.yml
- filename: reputation-summary-api-openapi.yml
  format: yaml
  label: Reputation Summary API
  slug: reputation-summary-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reputation/refs/heads/main/openapi/reputation-summary-api-openapi.yml
- filename: reputation-surveys-api-openapi.yml
  format: yaml
  label: Reputation Surveys API
  slug: reputation-surveys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reputation/refs/heads/main/openapi/reputation-surveys-api-openapi.yml
- filename: reputation-tenants-api-openapi.yml
  format: yaml
  label: Reputation Tenants API
  slug: reputation-tenants-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reputation/refs/heads/main/openapi/reputation-tenants-api-openapi.yml
- filename: reputation-tickets-api-openapi.yml
  format: yaml
  label: Reputation Tickets API
  slug: reputation-tickets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reputation/refs/heads/main/openapi/reputation-tickets-api-openapi.yml
- filename: reputation-users-api-openapi.yml
  format: yaml
  label: Reputation Users API
  slug: reputation-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reputation/refs/heads/main/openapi/reputation-users-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Reputation Authentication
name_suffix: Authentication
oauth_flows: []
overview: Reputation secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Reputation
provider_slug: reputation
scheme_count: 1
schemes:
- description: API key for authentication. For agency accounts, also include X-TENANT-ID header.
  in: header
  name: ApiKeyAuth
  parameter: X-API-KEY
  sources:
  - openapi/reputation-api-openapi.yml
  type: apiKey
slug: reputation-authentication
source_filename: reputation-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/reputation-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-API-KEY\n  description: API key for authentication. For agency accounts, also include X-TENANT-ID header.\n  sources:\n  - openapi/reputation-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/reputation/refs/heads/main/authentication/reputation-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Reputation Management
- Online Reviews
- Business Listings
- Surveys
- Social Listening
- Competitive Intelligence
- Customer Experience
- Local SEO
---
