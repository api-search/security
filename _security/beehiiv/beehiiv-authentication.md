---
api_key_in: []
api_specs:
- filename: beehiiv-openapi.yml
  format: yaml
  label: beehiiv Publications API
  slug: beehiiv-publications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/beehiiv/refs/heads/main/openapi/beehiiv-openapi.yml
- filename: beehiiv-openapi.yml
  format: yaml
  label: beehiiv Subscriptions API
  slug: beehiiv-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/beehiiv/refs/heads/main/openapi/beehiiv-openapi.yml
- filename: beehiiv-openapi.yml
  format: yaml
  label: beehiiv Posts API
  slug: beehiiv-posts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/beehiiv/refs/heads/main/openapi/beehiiv-openapi.yml
- filename: beehiiv-openapi.yml
  format: yaml
  label: beehiiv Automations API
  slug: beehiiv-automations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/beehiiv/refs/heads/main/openapi/beehiiv-openapi.yml
- filename: beehiiv-openapi.yml
  format: yaml
  label: beehiiv Custom Fields API
  slug: beehiiv-custom-fields-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/beehiiv/refs/heads/main/openapi/beehiiv-openapi.yml
- filename: beehiiv-openapi.yml
  format: yaml
  label: beehiiv Segments API
  slug: beehiiv-segments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/beehiiv/refs/heads/main/openapi/beehiiv-openapi.yml
- filename: beehiiv-openapi.yml
  format: yaml
  label: beehiiv Tiers API
  slug: beehiiv-tiers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/beehiiv/refs/heads/main/openapi/beehiiv-openapi.yml
- filename: beehiiv-openapi.yml
  format: yaml
  label: beehiiv Polls API
  slug: beehiiv-polls-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/beehiiv/refs/heads/main/openapi/beehiiv-openapi.yml
- filename: beehiiv-openapi.yml
  format: yaml
  label: beehiiv Webhooks API
  slug: beehiiv-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/beehiiv/refs/heads/main/openapi/beehiiv-openapi.yml
- filename: beehiiv-openapi.yml
  format: yaml
  label: beehiiv Newsletter Lists API
  slug: beehiiv-newsletter-lists-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/beehiiv/refs/heads/main/openapi/beehiiv-openapi.yml
- filename: beehiiv-openapi.yml
  format: yaml
  label: beehiiv Referral Program API
  slug: beehiiv-referral-program-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/beehiiv/refs/heads/main/openapi/beehiiv-openapi.yml
- filename: beehiiv-openapi.yml
  format: yaml
  label: beehiiv OAuth2 API
  slug: beehiiv-oauth2-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/beehiiv/refs/heads/main/openapi/beehiiv-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Beehiiv Authentication
name_suffix: Authentication
oauth_flows: []
overview: beehiiv secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: beehiiv
provider_slug: beehiiv
scheme_count: 1
schemes:
- name: BearerAuthScheme
  scheme: bearer
  sources:
  - openapi/beehiiv-openapi.yml
  type: http
slug: beehiiv-authentication
source_filename: beehiiv-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/beehiiv-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuthScheme\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/beehiiv-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/beehiiv/refs/heads/main/authentication/beehiiv-authentication.yml
summary_line: http · 1 scheme
tags:
- Newsletter
- Creator
- Email
- Subscription
- Publishing
- Media
- Advertising
---
