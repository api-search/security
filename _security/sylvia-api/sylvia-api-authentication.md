---
api_key_in: []
api_specs:
- filename: sylvia-api-live-api-openapi.yml
  format: yaml
  label: Sylvia API Live API
  slug: sylvia-api-live-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sylvia-api/refs/heads/main/openapi/sylvia-api-live-api-openapi.yml
- filename: sylvia-api-subreddits-api-openapi.yml
  format: yaml
  label: Sylvia API Subreddits API
  slug: sylvia-api-subreddits-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sylvia-api/refs/heads/main/openapi/sylvia-api-subreddits-api-openapi.yml
- filename: sylvia-api-users-api-openapi.yml
  format: yaml
  label: Sylvia API Users API
  slug: sylvia-api-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sylvia-api/refs/heads/main/openapi/sylvia-api-users-api-openapi.yml
- filename: sylvia-api-account-api-openapi.yml
  format: yaml
  label: Sylvia API Account API
  slug: sylvia-api-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sylvia-api/refs/heads/main/openapi/sylvia-api-account-api-openapi.yml
- filename: sylvia-api-billing-api-openapi.yml
  format: yaml
  label: Sylvia API Billing API
  slug: sylvia-api-billing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sylvia-api/refs/heads/main/openapi/sylvia-api-billing-api-openapi.yml
- filename: sylvia-api-discovery-api-openapi.yml
  format: yaml
  label: Sylvia API Discovery API
  slug: sylvia-api-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sylvia-api/refs/heads/main/openapi/sylvia-api-discovery-api-openapi.yml
- filename: sylvia-api-domains-api-openapi.yml
  format: yaml
  label: Sylvia API Domains API
  slug: sylvia-api-domains-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sylvia-api/refs/heads/main/openapi/sylvia-api-domains-api-openapi.yml
- filename: sylvia-api-health-api-openapi.yml
  format: yaml
  label: Sylvia API Health API
  slug: sylvia-api-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sylvia-api/refs/heads/main/openapi/sylvia-api-health-api-openapi.yml
- filename: sylvia-api-keys-api-openapi.yml
  format: yaml
  label: Sylvia API Keys API
  slug: sylvia-api-keys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sylvia-api/refs/heads/main/openapi/sylvia-api-keys-api-openapi.yml
- filename: sylvia-api-posts-comments-api-openapi.yml
  format: yaml
  label: Sylvia API Posts & Comments API
  slug: sylvia-api-posts-comments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sylvia-api/refs/heads/main/openapi/sylvia-api-posts-comments-api-openapi.yml
- filename: sylvia-api-search-api-openapi.yml
  format: yaml
  label: Sylvia API Search API
  slug: sylvia-api-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sylvia-api/refs/heads/main/openapi/sylvia-api-search-api-openapi.yml
- filename: sylvia-api-templates-api-openapi.yml
  format: yaml
  label: Sylvia API Templates API
  slug: sylvia-api-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sylvia-api/refs/heads/main/openapi/sylvia-api-templates-api-openapi.yml
auth_types: []
description: API key authentication, read from the provider-published specification.
kind: authentication
layout: security
method: searched
name: Sylvia Api Authentication
name_suffix: Authentication
oauth_flows: []
overview: Sylvia API declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Sylvia API
provider_slug: sylvia-api
scheme_count: 1
schemes:
- id: ApiKeyAuth
  in: header
  name: X-API-Key
  type: apiKey
slug: sylvia-api-authentication
source_filename: sylvia-api-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-04'\nmethod: searched\nstatus: published\nsource: https://sylvia-api.com/openapi.json\ndescription: API key authentication, read from the provider-published specification.\nverified: '2026-08-04'\nschemes:\n- id: ApiKeyAuth\n  type: apiKey\n  in: header\n  name: X-API-Key\nevidence:\n- url: https://sylvia-api.com/openapi.json\n  status: 200\n  note: distinct document — differs from the site-wide HTML catch-all\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sylvia-api/refs/heads/main/authentication/sylvia-api-authentication.yml
summary_line: 1 scheme
tags:
- Reddit
- Social
- Data
- Search
- Comments
- Research
- Content
- Datasets
---
