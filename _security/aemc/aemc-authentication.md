---
api_key_in: []
api_specs:
- filename: aemc-energy-rules-openapi-derived.yml
  format: yaml
  label: AEMC Energy Rules API
  slug: aemc-energy-rules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aemc/refs/heads/main/openapi/aemc-energy-rules-openapi-derived.yml
auth_types:
- none
description: ''
kind: authentication
layout: security
method: probed
name: Aemc Authentication
name_suffix: Authentication
oauth_flows: []
overview: Australian Energy Market Commission secures its APIs with none across 0 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Australian Energy Market Commission
provider_slug: aemc
scheme_count: 0
schemes: []
slug: aemc-authentication
source_filename: aemc-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-27'\nmethod: probed\nsource: live anonymous probes of https://energy-rules.aemc.gov.au/api/v1 on 2026-07-27\nsummary:\n  types: [none]\n  api_key_in: []\n  oauth2_flows: []\n  anonymous_read: true\nnote: >-\n  The AEMC Energy Rules API requires no authentication of any kind for read access. Every endpoint\n  in openapi/aemc-energy-rules-openapi-derived.yml was called anonymously on 2026-07-27 with no\n  key, no bearer token, no session cookie and no CSRF header, and returned HTTP 200 with data. The\n  spec therefore declares no securitySchemes — that is the real contract, not an omission.\nschemes: []\nobservations:\n- name: preview-token\n  kind: query parameter\n  parameter: previewToken\n  applies_to: [listRuleVersions, getRuleContent, searchRuleVersion]\n  description: >-\n    An editorial preview token accepted as a query parameter on several read endpoints, used by\n    AEMC's internal rule-approval workflow to view unapproved rule versions. It is\
  \ not obtainable\n    or usable anonymously and is not an end-user authentication mechanism.\n  probed: false\n- name: administrative-approval-route\n  kind: token-in-path\n  path_pattern: /api/v1/{type}/{version}/approve/{token}\n  description: >-\n    A state-changing approval route present in AEMC's production JavaScript bundle, guarded by a\n    token in the path. Deliberately NOT probed and deliberately not modelled in the OpenAPI. Noted\n    here because a token-in-URL approval link is a security-relevant design observation, not\n    because it is available for use.\n  probed: false\naemc_website:\n  host: www.aemc.gov.au\n  scheme: none\n  detail: >-\n    The AEMC corporate site (Drupal) publishes no protected API surface;\n    /.well-known/openid-configuration and /.well-known/oauth-authorization-server return 404\n    (re-probed 2026-07-27).\nrelated_regimes:\n  note: >-\n    For consumer energy data in Australia the authentication model that matters is the Consumer\n    Data\
  \ Right (OAuth2/OIDC + mTLS under the Consumer Data Standards), implemented by retailers and\n    AEMO — not by AEMC. See review.yml.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aemc/refs/heads/main/authentication/aemc-authentication.yml
summary_line: none · 0 schemes
tags:
- Energy
- Australia
- Energy Markets
- Electricity
- Gas
- Utilities
- Regulation
- Smart Metering
- Consumer Data Right
- Government
- Legal
- Rules
---
