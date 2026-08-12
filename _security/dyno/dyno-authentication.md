---
api_key_in:
- header
api_specs:
- filename: dyno-phi-openapi.yml
  format: yaml
  label: Dyno Phi — Protein Design API
  slug: dyno-phi-protein-design-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dyno/refs/heads/main/openapi/dyno-phi-openapi.yml
auth_types:
- apiKey
- http-bearer
- oidc-session
description: 'Authentication profile for the Dyno Phi Protein Design API. Derived from the provider''s OpenAPI 3.1.0 document, its first-party CLI source (github.com/dynotx/phi-cli), and a live unauthenticated probe of the API. IMPORTANT: the spec declares NO components.securitySchemes and no top-level security[] block — the API key is modelled as an ordinary optional header PARAMETER on every operation. The real, enforced mechanism was confirmed by probing the live API.'
kind: authentication
layout: security
method: searched
name: Dyno Authentication
name_suffix: Authentication
oauth_flows: []
overview: Dyno secures its APIs with apiKey, http-bearer, and oidc-session across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Dyno
provider_slug: dyno
scheme_count: 3
schemes:
- evidence: GET https://api.dyno-agents.app/v1/phi/jobs/ with no credentials returns HTTP 401 {"detail":"Missing API key. Provide an x-api-key header."}. The first-party CLI sends the header as `x-api-key` on every request.
  in: header
  key_prefix: ak_
  name: x-api-key
  note: 'Declared in the OpenAPI only as an optional header parameter (`required: false`) on all 80 operations, which understates the contract — the header is in fact mandatory.'
  parameter: x-api-key
  required: true
  source: live probe + github.com/dynotx/phi-cli/src/phi/api.py
  type: apiKey
- evidence: '"All endpoints require an API key supplied as `Authorization: Bearer <key>` or a Clerk session token."'
  name: Authorization Bearer
  note: Documented in the spec description but contradicted by the live 401, which names only x-api-key. Treat x-api-key as authoritative; Bearer may be an accepted alternate. Not independently confirmed.
  scheme: bearer
  source: openapi info.description
  type: http
- discovery: none
  evidence: The open-source notice lists Clerk (commercial licence) in the platform stack; the OpenAPI description states organisation ID is derived automatically from Clerk tokens. Used by the design.dynotx.com dashboard.
  name: Clerk session token
  note: No /.well-known/openid-configuration is served on any Dyno host, so the issuer is not machine-discoverable. See well-known/dyno-well-known.yml.
  provider: Clerk
  source: https://design.dynotx.com/open-source
  type: openIdConnect
slug: dyno-authentication
source_filename: dyno-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-10'\nmethod: searched\nsource: https://api.dyno-agents.app/v1/phi/openapi.json\ndocs: https://design.dynotx.com/cli\ndescription: >-\n  Authentication profile for the Dyno Phi Protein Design API. Derived from the\n  provider's OpenAPI 3.1.0 document, its first-party CLI source\n  (github.com/dynotx/phi-cli), and a live unauthenticated probe of the API.\n  IMPORTANT: the spec declares NO components.securitySchemes and no top-level\n  security[] block — the API key is modelled as an ordinary optional header\n  PARAMETER on every operation. The real, enforced mechanism was confirmed by\n  probing the live API.\nsummary:\n  types: [apiKey, http-bearer, oidc-session]\n  api_key_in: [header]\n  oauth2_flows: []\n  spec_declares_security_schemes: false\n  enforced: true\nschemes:\n- name: x-api-key\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  required: true\n  key_prefix: ak_\n  source: live probe + github.com/dynotx/phi-cli/src/phi/api.py\n  evidence:\
  \ >-\n    GET https://api.dyno-agents.app/v1/phi/jobs/ with no credentials returns\n    HTTP 401 {\"detail\":\"Missing API key. Provide an x-api-key header.\"}. The\n    first-party CLI sends the header as `x-api-key` on every request.\n  note: >-\n    Declared in the OpenAPI only as an optional header parameter\n    (`required: false`) on all 80 operations, which understates the contract —\n    the header is in fact mandatory.\n- name: Authorization Bearer\n  type: http\n  scheme: bearer\n  source: openapi info.description\n  evidence: >-\n    \"All endpoints require an API key supplied as `Authorization: Bearer <key>`\n    or a Clerk session token.\"\n  note: >-\n    Documented in the spec description but contradicted by the live 401, which\n    names only x-api-key. Treat x-api-key as authoritative; Bearer may be an\n    accepted alternate. Not independently confirmed.\n- name: Clerk session token\n  type: openIdConnect\n  provider: Clerk\n  source: https://design.dynotx.com/open-source\n\
  \  evidence: >-\n    The open-source notice lists Clerk (commercial licence) in the platform\n    stack; the OpenAPI description states organisation ID is derived\n    automatically from Clerk tokens. Used by the design.dynotx.com dashboard.\n  discovery: none\n  note: >-\n    No /.well-known/openid-configuration is served on any Dyno host, so the\n    issuer is not machine-discoverable. See well-known/dyno-well-known.yml.\ntenancy_headers:\n- name: X-Organization-ID\n  required_when: static API key callers\n  source: openapi info.description\n  note: \"\\\"Organisation ID is derived automatically from Clerk tokens; static-key callers must include X-Organization-ID.\\\"\"\n- name: X-User-ID\n  required: false\n  source: openapi parameters + phi-cli (DYNO_USER_ID env var)\nkey_management:\n  issue_url: https://design.dynotx.com/dashboard/settings\n  path: Settings -> API keys\n  env_var: DYNO_API_KEY\n  base_url_env_var: DYNO_API_BASE_URL\n  local_cache: .phi/state.json (written by the\
  \ CLI on first use)\n  rotation_policy: not published\n  expiry_policy: not published\n  scoping: not published (no scopes/permissions surface)\ngaps_to_report_upstream:\n- >-\n  No components.securitySchemes in the OpenAPI — every generated client and\n  every agent reading the spec will treat auth as optional. Adding an apiKey\n  scheme named x-api-key plus a top-level security requirement is a one-line fix.\n- >-\n  The spec description documents an `Authorization: Bearer` scheme but the\n  server answers with an x-api-key challenge; the two disagree.\n- No 401 or 403 response is declared on any of the 80 operations.\nx-evidence:\n  fetched: '2026-08-10'\n  urls:\n  - {url: 'https://api.dyno-agents.app/v1/phi/openapi.json', http_status: 200}\n  - {url: 'https://api.dyno-agents.app/v1/phi/jobs/', http_status: 401}\n  - {url: 'https://api.dyno-agents.app/v1/phi/auth/me', http_status: 401}\n  - {url: 'https://raw.githubusercontent.com/dynotx/phi-cli/main/src/phi/config.py', http_status:\
  \ 200}\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dyno/refs/heads/main/authentication/dyno-authentication.yml
summary_line: apiKey/http-bearer/oidc-session · 3 schemes
tags:
- Company
- Biotechnology
- Gene Therapy
- Genetic Medicine
- Gene Delivery
- AAV Capsid
- Artificial Intelligence
- Machine Learning
- Drug Discovery
- Healthcare
- Protein Design
- Protein Structure Prediction
- Bioinformatics
- Computational Biology
- Agentic AI
- Life Sciences
---
