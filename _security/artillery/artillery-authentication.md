---
anonymous_access: false
api_key_in:
- cli-flag
- environment-variable
- header
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Artillery Authentication
name_suffix: Authentication
oauth_flows: []
overview: Artillery secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Artillery
provider_slug: artillery
scheme_count: 2
schemes:
- alt_parameter: ARTILLERY_CLOUD_API_KEY
  in: cli-flag
  key_prefix: a9_
  key_prefix_evidence: https://www.artillery.io/docs/reference/stash — published example "ARTILLERY_CLOUD_API_KEY=a9_yourApiKey node seed-data.ts"
  name: ArtilleryCloudApiKey
  obtained_from: Artillery Cloud dashboard settings at https://app.artillery.io
  parameter: --key
  sources:
  - docs
  type: apiKey
  used_by:
  - artillery run --record --key <key>  (record a test run to Artillery Cloud)
  - Stash API (persistent key-value store; client auto-configured from the same key)
  - '@artilleryio/playwright-reporter (Playwright E2E reporting into Artillery Cloud)'
- in: header
  name: ArtilleryCloudSessionToken
  observation: Anonymous requests to any path under https://app.artillery.io/api return HTTP 401 with the body {"error":{"data":{"message":"Missing auth token","code":401,"type":"ServerError"}}}. The token name and format are not published; the Cloud API is an undocumented, authenticated-only surface.
  observed: true
  scheme: bearer
  sources:
  - live probe 2026-09-07
  type: http
slug: artillery-authentication
source_filename: artillery-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-07'\nmethod: searched\nsource: >-\n  https://www.artillery.io/docs/reference/stash, https://www.artillery.io/docs/reference/cli/run,\n  https://www.artillery.io/pricing, https://www.artillery.io/changelog, plus live anonymous\n  probes of https://app.artillery.io/api\ndocs: https://www.artillery.io/docs/reference/cli/run\nnote: >-\n  DERIVED FROM DOCS AND LIVE PROBES, NOT FROM A SPEC — Artillery publishes no OpenAPI, so there\n  are no securitySchemes to aggregate. What is recorded below is what the provider documents\n  and what the live endpoint actually answers.\nsummary:\n  types: [apiKey]\n  api_key_in: [cli-flag, environment-variable, header]\n  oauth2_flows: []\n  federation: [oidc, saml]\n  provisioning: [scim]\nschemes:\n- name: ArtilleryCloudApiKey\n  type: apiKey\n  in: cli-flag\n  parameter: --key\n  alt_parameter: ARTILLERY_CLOUD_API_KEY\n  key_prefix: a9_\n  key_prefix_evidence: >-\n    https://www.artillery.io/docs/reference/stash — published\
  \ example\n    \"ARTILLERY_CLOUD_API_KEY=a9_yourApiKey node seed-data.ts\"\n  obtained_from: Artillery Cloud dashboard settings at https://app.artillery.io\n  used_by:\n  - artillery run --record --key <key>  (record a test run to Artillery Cloud)\n  - Stash API (persistent key-value store; client auto-configured from the same key)\n  - '@artilleryio/playwright-reporter (Playwright E2E reporting into Artillery Cloud)'\n  sources: [docs]\n- name: ArtilleryCloudSessionToken\n  type: http\n  scheme: bearer\n  in: header\n  observed: true\n  observation: >-\n    Anonymous requests to any path under https://app.artillery.io/api return HTTP 401 with the\n    body {\"error\":{\"data\":{\"message\":\"Missing auth token\",\"code\":401,\"type\":\"ServerError\"}}}.\n    The token name and format are not published; the Cloud API is an undocumented,\n    authenticated-only surface.\n  sources: [live probe 2026-09-07]\nfederation:\n- name: Enterprise SSO\n  protocols: [oidc, saml]\n  provisioning: scim\n\
  \  self_service: true\n  evidence: >-\n    Pricing page lists \"Enterprise SSO (OIDC & SAML), audit logs, custom MSA, and support SLAs\"\n    as an add-on from $1199/month; the changelog entry of 2026-07-29 announces self-service SSO\n    and SCIM onboarding from Settings -> SSO in Artillery Cloud.\n  docs: https://www.artillery.io/pricing\npublic_surface_note: >-\n  There is no anonymous or public-read surface on the Artillery Cloud API. Everything an agent\n  or integrator can do without credentials is documentation: /llms.txt, the .md docs mirror, the\n  public GitHub org, and the npm packages.\nx-evidence:\n  fetched: '2026-09-07'\n  probes:\n  - {url: 'https://app.artillery.io/api/openapi.json', status: 401}\n  - {url: 'https://app.artillery.io/api/graphql', status: 401}\n  - {url: 'https://www.artillery.io/docs/reference/stash', status: 200}\n  - {url: 'https://www.artillery.io/pricing', status: 200}\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/artillery/refs/heads/main/authentication/artillery-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Load Testing
- Performance Testing
- Open-Source
- Testing
- DevOps
- Node.js
---
