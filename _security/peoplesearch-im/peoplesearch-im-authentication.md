---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: peoplesearch-im-credits-api-openapi.yml
  format: yaml
  label: PeopleSearch.im Credits API
  slug: peoplesearch-im-credits-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/peoplesearch-im/refs/heads/main/openapi/peoplesearch-im-credits-api-openapi.yml
- filename: peoplesearch-im-deliver-api-openapi.yml
  format: yaml
  label: PeopleSearch.im Deliver API
  slug: peoplesearch-im-deliver-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/peoplesearch-im/refs/heads/main/openapi/peoplesearch-im-deliver-api-openapi.yml
- filename: peoplesearch-im-email-api-openapi.yml
  format: yaml
  label: PeopleSearch.im Email API
  slug: peoplesearch-im-email-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/peoplesearch-im/refs/heads/main/openapi/peoplesearch-im-email-api-openapi.yml
- filename: peoplesearch-im-reveal-api-openapi.yml
  format: yaml
  label: PeopleSearch.im Reveal API
  slug: peoplesearch-im-reveal-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/peoplesearch-im/refs/heads/main/openapi/peoplesearch-im-reveal-api-openapi.yml
- filename: peoplesearch-im-search-api-openapi.yml
  format: yaml
  label: PeopleSearch.im Search API
  slug: peoplesearch-im-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/peoplesearch-im/refs/heads/main/openapi/peoplesearch-im-search-api-openapi.yml
- filename: peoplesearch-im-tools-api-openapi.yml
  format: yaml
  label: PeopleSearch.im Tools API
  slug: peoplesearch-im-tools-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/peoplesearch-im/refs/heads/main/openapi/peoplesearch-im-tools-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: derived
name: Peoplesearch Im Authentication
name_suffix: Authentication
oauth_flows: []
overview: PeopleSearch.im secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: PeopleSearch.im
provider_slug: peoplesearch-im
scheme_count: 2
schemes:
- bearerFormat: sk_sift_…
  description: A PeopleSearch.im API key, created at /developers.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/peoplesearch-im-openapi.json
  type: http
- description: The same PeopleSearch.im API key (sk_sift_…), sent as a header.
  in: header
  name: apiKeyHeader
  parameter: X-API-Key
  sources:
  - openapi/peoplesearch-im-openapi.json
  type: apiKey
slug: peoplesearch-im-authentication
source_filename: peoplesearch-im-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-12'\nmethod: derived\nsource: openapi/peoplesearch-im-openapi.json\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: sk_sift_…\n  description: A PeopleSearch.im API key, created at /developers.\n  sources:\n  - openapi/peoplesearch-im-openapi.json\n- name: apiKeyHeader\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  description: The same PeopleSearch.im API key (sk_sift_…), sent as a header.\n  sources:\n  - openapi/peoplesearch-im-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/peoplesearch-im/refs/heads/main/authentication/peoplesearch-im-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Company
- People Search
- Email Lookup
- AI
- SaaS
---
