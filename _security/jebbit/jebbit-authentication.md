---
api_key_in: []
api_specs:
- filename: jebbit-auth-api-openapi.yml
  format: yaml
  label: Jebbit Auth API
  slug: jebbit-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jebbit/refs/heads/main/openapi/jebbit-auth-api-openapi.yml
- filename: jebbit-businesses-api-openapi.yml
  format: yaml
  label: Jebbit Businesses API
  slug: jebbit-businesses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jebbit/refs/heads/main/openapi/jebbit-businesses-api-openapi.yml
- filename: jebbit-campaigns-api-openapi.yml
  format: yaml
  label: Jebbit Campaigns API
  slug: jebbit-campaigns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jebbit/refs/heads/main/openapi/jebbit-campaigns-api-openapi.yml
- filename: jebbit-feed-columns-api-openapi.yml
  format: yaml
  label: Jebbit Feed Columns API
  slug: jebbit-feed-columns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jebbit/refs/heads/main/openapi/jebbit-feed-columns-api-openapi.yml
- filename: jebbit-feed-rows-api-openapi.yml
  format: yaml
  label: Jebbit Feed Rows API
  slug: jebbit-feed-rows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jebbit/refs/heads/main/openapi/jebbit-feed-rows-api-openapi.yml
- filename: jebbit-feeds-api-openapi.yml
  format: yaml
  label: Jebbit Feeds API
  slug: jebbit-feeds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jebbit/refs/heads/main/openapi/jebbit-feeds-api-openapi.yml
- filename: jebbit-integration-historic-backfills-api-openapi.yml
  format: yaml
  label: Jebbit Integration Historic Backfills API
  slug: jebbit-integration-historic-backfills-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jebbit/refs/heads/main/openapi/jebbit-integration-historic-backfills-api-openapi.yml
- filename: jebbit-integration-mappings-api-openapi.yml
  format: yaml
  label: Jebbit Integration Mappings API
  slug: jebbit-integration-mappings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jebbit/refs/heads/main/openapi/jebbit-integration-mappings-api-openapi.yml
- filename: jebbit-integrations-api-openapi.yml
  format: yaml
  label: Jebbit Integrations API
  slug: jebbit-integrations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jebbit/refs/heads/main/openapi/jebbit-integrations-api-openapi.yml
- filename: jebbit-launch-links-api-openapi.yml
  format: yaml
  label: Jebbit Launch Links API
  slug: jebbit-launch-links-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jebbit/refs/heads/main/openapi/jebbit-launch-links-api-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Jebbit Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Jebbit secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Jebbit
provider_slug: jebbit
scheme_count: 1
schemes:
- audience: public-api
  bearerFormat: JWT
  flow: clientCredentials
  header: 'Authorization: Bearer <jwt>'
  name: JWT
  scopes:
  - read
  - write
  - delete
  - read:integration
  - write:integration
  sources:
  - openapi/jebbit-openapi-original.json
  - docs
  tokenUrl: https://auth.jebbit.com/oauth/token
  type: oauth2
slug: jebbit-authentication
source_filename: jebbit-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: openapi/jebbit-openapi-original.json\ndocs: https://support-experiences.blueconic.com/en/articles/246971-api-overview\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\n  token_format: JWT\nnote: 'The OpenAPI models auth as http/bearer(JWT); the docs specify the real mechanism: OAuth 2.0 client_credentials\n  against an Auth0 tenant (auth.jebbit.com), audience \"public-api\", 24h JWT. A x-jebbit-business header\n  scopes multi-business tokens.'\nschemes:\n- name: JWT\n  type: oauth2\n  flow: clientCredentials\n  bearerFormat: JWT\n  tokenUrl: https://auth.jebbit.com/oauth/token\n  audience: public-api\n  header: 'Authorization: Bearer <jwt>'\n  scopes:\n  - read\n  - write\n  - delete\n  - read:integration\n  - write:integration\n  sources:\n  - openapi/jebbit-openapi-original.json\n  - docs\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/jebbit/refs/heads/main/authentication/jebbit-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Company
- Interactive Experiences
- Zero-Party Data
- First-Party Data
- Marketing
- Quizzes
- Product Feeds
- Webhooks
- Customer Data
- JSON:API
---
