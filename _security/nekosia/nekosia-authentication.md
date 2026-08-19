---
api_key_in: []
auth_types:
- none
description: ''
kind: authentication
layout: security
method: searched
name: Nekosia Authentication
name_suffix: Authentication
oauth_flows: []
overview: Nekosia API secures its APIs with none across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Nekosia API
provider_slug: nekosia
scheme_count: 1
schemes:
- description: 'The Nekosia REST API requires no authorization key, token, header or account. The provider states this as a deliberate product decision: "The API does not require authorization keys or tokens, so you don''t need to register to use it. This increases accessibility and convenience." Verified — GET https://api.nekosia.cat/api/v1/images/catgirl returns 200 with a full image payload on a bare request carrying no credentials.'
  name: none
  sources:
  - https://nekosia.cat/documentation?page=introduction
  - live probe 2026-08-19
  type: none
slug: nekosia-authentication
source_filename: nekosia-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-19'\nmethod: searched\nsource: >-\n  https://nekosia.cat/documentation?page=introduction (\"No API Key Required\" section) and\n  https://nekosia.cat/documentation?page=getting-started, verified by live unauthenticated calls to\n  https://api.nekosia.cat/api/v1/* on 2026-08-19 which returned 200 with no credential of any kind.\ndocs: https://nekosia.cat/documentation?page=introduction\nchecked: '2026-08-19'\nsummary:\n  types: [none]\n  api_key_in: []\n  oauth2_flows: []\n  authentication_required: false\n  registration_required: false\nschemes:\n  - name: none\n    type: none\n    description: >-\n      The Nekosia REST API requires no authorization key, token, header or account. The provider\n      states this as a deliberate product decision: \"The API does not require authorization keys or\n      tokens, so you don't need to register to use it. This increases accessibility and\n      convenience.\" Verified — GET https://api.nekosia.cat/api/v1/images/catgirl\
  \ returns 200 with a\n      full image payload on a bare request carrying no credentials.\n    sources:\n      - https://nekosia.cat/documentation?page=introduction\n      - live probe 2026-08-19\ndocumented: true\ndocumented_note: >-\n  This is a documented authentication MODEL, not a missing one. The provider names the model, says\n  why, and the docs' getting-started flow is a credential-free curl. That is the thing the\n  `authentication_documented` check exists to reward — a consumer knows exactly what to send.\nidentity_and_quota:\n  identity_unit: client IP address\n  note: >-\n    With no key there is no caller identity, so everything that would normally attach to a key\n    attaches to the source IP instead: the 300-requests-per-5-minutes budget, abuse blocking, and\n    IP-keyed sessions. There is no mechanism to identify yourself for a higher allowance.\n  consequence_for_agents: >-\n    Agents running from shared or serverless egress share one rate-limit budget and one IP-keyed\n\
  \    session window with every other caller on that address. Use `session=id` with a per-end-user\n    identifier rather than `session=ip`.\n  see: rate-limits/nekosia-rate-limits.yml\nwebsite_authentication:\n  applies_to: nekosia.cat / Nekosia Booru accounts — NOT the API\n  mechanisms:\n    - password login with email-based password reset (added 2026-06-17)\n    - social login including X (Twitter) via OAuth2 (moved to OAuth2 on 2026-04-02, fixed 2026-05-10)\n  note: >-\n    The website has accounts, roles and OAuth2 social login for the Booru. None of it grants or\n    affects API access, and no OAuth authorization-server metadata is published\n    (/.well-known/oauth-authorization-server 404s on every host). Recorded so a later round does\n    not mistake the site login for an API auth surface.\n  source: https://nekosia.cat/documentation?page=changelog\nscopes:\n  applicable: false\n  note: >-\n    No OAuth on the API surface, therefore no scope model and no scopes/ artifact. The\n\
  \    derive-oauth-scopes step is not applicable to this provider.\ntransport_security:\n  https_required: true\n  hsts: 'max-age=31536000; includeSubDomains; preload'\n  tls_version_observed: TLSv1.3\n  see: security/nekosia-domain-security.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nekosia/refs/heads/main/authentication/nekosia-authentication.yml
summary_line: none · 1 scheme
tags:
- anime
- neko
- api
- nekos
- neko api
- booru
- image
- media
- entertainment
- images
- free api
- open access
---
