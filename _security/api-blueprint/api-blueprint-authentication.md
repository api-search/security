---
api_key_in: []
api_specs:
- filename: api-blueprint-parsing-service-openapi.yml
  format: yaml
  label: API Blueprint API
  slug: api-blueprint-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/api-blueprint/refs/heads/main/openapi/api-blueprint-parsing-service-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
method: probed
name: Api Blueprint Authentication
name_suffix: Authentication
oauth_flows: []
overview: API Blueprint declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: API Blueprint
provider_slug: api-blueprint
scheme_count: 0
schemes: []
slug: api-blueprint-authentication
source_filename: api-blueprint-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-02'\nmethod: probed\nsource: >-\n  derive-authentication.py produced nothing because the provider's contract\n  declares no securitySchemes — correctly, because the API has no\n  authentication at all. This file records that as a positive finding rather\n  than an absence. Established by unauthenticated live probes of\n  https://api.apiblueprint.org on 2026-09-02 and by reading the provider's API\n  Blueprint contract in apib/, which documents no credential of any kind.\nprovider: API Blueprint\nproviderId: api-blueprint\nsummary: >-\n  The API Blueprint parsing service is completely open. There is no API key, no\n  token, no OAuth flow, no sign-up and no account. Every operation was called\n  successfully on 2026-09-02 with no credential.\nschemes: []\nauthentication_required: false\nsignup_required: false\nschemes_detail:\n  - id: none\n    type: none\n    description: >-\n      No authentication. Confirmed by calling every operation anonymously:\n   \
  \   GET / -> 200; POST /parser with an API Blueprint body -> 200 with a parse\n      result; POST /validate -> 200; POST /transform -> 200. No 401 or 403 was\n      returned by any request during the pass.\ndiscovery:\n  - path: /.well-known/oauth-authorization-server\n    host: api.apiblueprint.org\n    status: 404\n  - path: /.well-known/openid-configuration\n    host: api.apiblueprint.org\n    status: 404\n  - path: /.well-known/oauth-protected-resource\n    host: api.apiblueprint.org\n    status: 404\n  - path: /.well-known/oauth-authorization-server\n    host: apiblueprint.org\n    status: 404\n  - path: /.well-known/openid-configuration\n    host: apiblueprint.org\n    status: 404\ntransport:\n  https: true\n  tls_version: TLSv1.2\n  hsts: false\n  note: >-\n    TLS observed at TLSv1.2 on api.apiblueprint.org (the marketing host\n    apiblueprint.org negotiates TLSv1.3). HSTS is not set on either host. See\n    security/api-blueprint-domain-security.yml.\nagent_note: >-\n  An agent\
  \ can call this API with no onboarding step whatsoever. That is the\n  strongest agent-access property in this profile and the weakest security one:\n  there is no way to attribute, meter or revoke a caller, and no rate limit is\n  published or observed.\nmaintainers:\n  - FN: Kin Lane\n    email: kin@apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/api-blueprint/refs/heads/main/authentication/api-blueprint-authentication.yml
summary_line: 0 schemes
tags:
- API Design
- Specification Language
- Markdown
- Documentation
- API Description Language
- Parsing
- Open Source
- Developer Tools
---
