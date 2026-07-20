---
api_key_in:
- header
api_specs:
- filename: koi-security-extensiontotal-openapi.yml
  format: yaml
  label: ExtensionTotal API
  slug: koi-security-extensiontotal
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/koi-security/refs/heads/main/openapi/koi-security-extensiontotal-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Koi Security Authentication
name_suffix: Authentication
oauth_flows: []
overview: Koi Security secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Koi Security
provider_slug: koi-security
scheme_count: 1
schemes:
- description: 'Organizational API key issued by Koi. Omit for free, rate-limited anonymous access. Koi''s guide

    documents the header case-insensitively as both `X-API-Key` and `x-api-key`.'
  in: header
  name: ApiKeyAuth
  parameter: X-API-Key
  sources:
  - openapi/koi-security-extensiontotal-openapi.yml
  type: apiKey
slug: koi-security-authentication
source_filename: koi-security-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: openapi/koi-security-extensiontotal-openapi.yml\ndocs: https://www.koi.ai/blog/6-6-uncover-hidden-risks-cisos-guide-to-using-extensiontotal-api-for-your-organization\nnotes: |\n  Koi's published ExtensionTotal API guide documents a single API-key header. There is no OAuth,\n  OIDC, or scope surface on the public API, so no scopes/ artifact is emitted. The Koi platform\n  console at docs.koi.ai sits behind an OIDC sign-in at auth.koi.security, but that flow is not\n  publicly documented and no discovery document is published.\nkey_issuance:\n  anonymous: Free, rate-limited access with no key.\n  organizational: API keys issued by Koi; documented as having no rate limit.\n  request_url: https://app.extensiontotal.com/sponsor\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  description: |-\n    Organizational API key issued by Koi.\
  \ Omit for free, rate-limited anonymous access. Koi's guide\n    documents the header case-insensitively as both `X-API-Key` and `x-api-key`.\n  sources:\n  - openapi/koi-security-extensiontotal-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/koi-security/refs/heads/main/authentication/koi-security-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Security
- Endpoint Security
- Supply Chain Security
- Browser Extensions
- Developer Tools
- Threat Intelligence
- MCP Security
- Risk Scoring
---
