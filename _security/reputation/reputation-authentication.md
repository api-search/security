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
method: searched
name: Reputation Authentication
name_suffix: Authentication
oauth_flows: []
overview: Reputation secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Reputation
provider_slug: reputation
scheme_count: 1
schemes:
- description: API key for authentication, applied globally to all 67 published operations. Issued only by a Reputation customer success manager — there is no self-serve key issuance, no key-management endpoint, and no documented rotation or expiry policy.
  in: header
  name: ApiKeyAuth
  parameter: X-API-KEY
  sources:
  - openapi/_original/reputation-api-openapi.yml
  type: apiKey
slug: reputation-authentication
source_filename: reputation-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: openapi/_original/reputation-api-openapi.yml\ndocs: https://apidocs.reputation.com/\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  oauth2_flows: []\n  applies_to_operations: 67\n  applies_to_operations_total: 67\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-API-KEY\n  description: >-\n    API key for authentication, applied globally to all 67 published operations. Issued only by a\n    Reputation customer success manager — there is no self-serve key issuance, no key-management\n    endpoint, and no documented rotation or expiry policy.\n  sources:\n  - openapi/_original/reputation-api-openapi.yml\ncompanion_headers:\n- name: X-TENANT-ID\n  required_when: >-\n    The API key is an Agency key. An Agency key manages resources across multiple client tenants,\n    and each request must name the target tenant so actions are scoped correctly.\n  omission_behaviour: >-\n    Returns HTTP\
  \ 404 \"Missing Tenant Id\" — not 401 or 400. Clients must special-case this.\n  source: https://apidocs.reputation.com/\nkey_lifecycle:\n  issuance: Contact your Reputation customer success manager.\n  self_serve: false\n  rotation_endpoint: null\n  expiry_documented: false\n  scopes: null\n  scope_note: >-\n    The API has no OAuth2 surface and therefore no scopes. Permission is carried entirely by the\n    key; a key either is or is not \"permitted the operation\" (HTTP 403). No scopes/ artifact is\n    emitted because there is nothing to enumerate.\ntransport:\n  tls_required: true\n  cipher_policy_published: true\n  cipher_policy_source: https://apidocs.reputation.com/\noauth_lookalike:\n  operation: get_credentials_oauth\n  path: /v3/credentials/oauth\n  note: >-\n    GET /v3/credentials/oauth reports the OAuth connection status of third-party review and social\n    sources connected to the account. It is NOT an OAuth flow for the Reputation API itself and must\n    not be read as\
  \ one.\nregions:\n- {region: US, host: 'https://api.reputation.com', docs: 'https://apidocs.reputation.com/'}\n- {region: EU, host: 'https://api-eu.reputation.com', docs: 'https://apidocs-eu.reputation.com/'}\nregion_note: A key issued in one data region is not valid in the other; US and EU are separated.\nexample:\n  curl: |\n    curl -H \"Content-Type: application/json\" \\\n         -H \"X-API-KEY: $ACCESS_TOKEN\" \\\n         -H \"X-TENANT-ID: $TENANT_ID\" \\\n         \"https://api.reputation.com/v3/locations\"\n  source: https://apidocs.reputation.com/\n"
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
