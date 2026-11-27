---
anonymous_access: false
api_key_in: []
api_specs:
- filename: tenderlead-co-uk-access-request-api-openapi.yml
  format: yaml
  label: TenderLead Access Request API
  slug: tenderlead-co-uk-access-request-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tenderlead-co-uk/openapi/tenderlead-co-uk-access-request-api-openapi.yml
- filename: tenderlead-co-uk-auth-api-openapi.yml
  format: yaml
  label: TenderLead Auth API
  slug: tenderlead-co-uk-auth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tenderlead-co-uk/openapi/tenderlead-co-uk-auth-api-openapi.yml
- filename: tenderlead-co-uk-briefs-api-openapi.yml
  format: yaml
  label: TenderLead Briefs API
  slug: tenderlead-co-uk-briefs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tenderlead-co-uk/openapi/tenderlead-co-uk-briefs-api-openapi.yml
- filename: tenderlead-co-uk-feedback-api-openapi.yml
  format: yaml
  label: TenderLead Feedback API
  slug: tenderlead-co-uk-feedback-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tenderlead-co-uk/openapi/tenderlead-co-uk-feedback-api-openapi.yml
- filename: tenderlead-co-uk-unsubscribe-api-openapi.yml
  format: yaml
  label: TenderLead Unsubscribe API
  slug: tenderlead-co-uk-unsubscribe-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tenderlead-co-uk/openapi/tenderlead-co-uk-unsubscribe-api-openapi.yml
- filename: tenderlead-co-uk-waitlist-api-openapi.yml
  format: yaml
  label: TenderLead Waitlist API
  slug: tenderlead-co-uk-waitlist-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tenderlead-co-uk/openapi/tenderlead-co-uk-waitlist-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: TenderLead Authentication
name_suffix: Authentication
oauth_flows: []
overview: TenderLead secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: TenderLead
provider_slug: tenderlead-co-uk
scheme_count: 1
schemes:
- description: 'Use a read-only token from Settings > API access in the Authorization: Bearer header. The daily brief requires briefs:read. The current narrowest token option grants briefs:read and tenders:read. Tokens are account-scoped, revocable and expire after 90 days. Never put a token in a URL or public example.'
  name: apiToken
  scheme: bearer
  sources:
  - openapi/tenderlead-co-uk-openapi.json
  type: http
slug: tenderlead-co-uk-authentication
source_filename: tenderlead-co-uk-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-26'\nmethod: derived\nsource: openapi/tenderlead-co-uk-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: apiToken\n  type: http\n  scheme: bearer\n  description: 'Use a read-only token from Settings > API access in the Authorization: Bearer\n    header. The daily brief requires briefs:read. The current narrowest token option grants\n    briefs:read and tenders:read. Tokens are account-scoped, revocable and expire after 90 days.\n    Never put a token in a URL or public example.'\n  sources:\n  - openapi/tenderlead-co-uk-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/tenderlead-co-uk/authentication/tenderlead-co-uk-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Tender
- UK
- Procurement
- SaaS
---
