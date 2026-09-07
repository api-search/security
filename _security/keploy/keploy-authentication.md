---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: keploy-cloud-api-openapi.yaml
  format: yaml
  label: Keploy Cloud API
  slug: keploy-cloud-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/keploy/refs/heads/main/openapi/keploy-cloud-api-openapi.yaml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Keploy Authentication
name_suffix: Authentication
oauth_flows: []
overview: Keploy secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Keploy
provider_slug: keploy
scheme_count: 1
schemes:
- alternate_header: 'Authorization: Bearer kep_...'
  description: 'Scoped Personal Access Token (`kep_`-prefixed), generated from the Keploy Console (Settings > API Keys). Accepted either as `X-API-Key: kep_...` or as `Authorization: Bearer kep_...` — both header forms are documented in the Public API reference.'
  in: header
  key_management:
    console: https://app.keploy.io
    create: POST /api-keys (requires an existing admin-scoped key; supports name, scopes, ttl_days)
    list: GET /api-keys
    revoke: DELETE /api-keys/{keyId}
  key_prefix: kep_
  name: apiKeyAuth
  parameter: X-API-Key
  scopes:
    admin: Everything in write + API key management + app deletion
    read: All GET endpoints (view apps, suites, runs, jobs)
    write: Everything in read + create, update, delete, generate, run
  sources:
  - openapi/keploy-cloud-api-openapi.yaml
  - https://keploy.io/docs/running-keploy/public-api/
  type: apiKey
slug: keploy-authentication
source_filename: keploy-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-03'\nmethod: searched\nsource: openapi/keploy-cloud-api-openapi.yaml\ndocs: https://keploy.io/docs/running-keploy/api-testing-auth-setup/\nreference: https://keploy.io/docs/running-keploy/public-api/\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  description: >-\n    Scoped Personal Access Token (`kep_`-prefixed), generated from the Keploy\n    Console (Settings > API Keys). Accepted either as `X-API-Key: kep_...` or\n    as `Authorization: Bearer kep_...` — both header forms are documented in\n    the Public API reference.\n  alternate_header: 'Authorization: Bearer kep_...'\n  key_prefix: kep_\n  scopes:\n    read: All GET endpoints (view apps, suites, runs, jobs)\n    write: Everything in read + create, update, delete, generate, run\n    admin: Everything in write + API key management + app deletion\n  key_management:\n    create: POST /api-keys (requires\
  \ an existing admin-scoped key; supports name, scopes, ttl_days)\n    list: GET /api-keys\n    revoke: DELETE /api-keys/{keyId}\n    console: https://app.keploy.io\n  sources:\n  - openapi/keploy-cloud-api-openapi.yaml\n  - https://keploy.io/docs/running-keploy/public-api/\nnotes: >-\n  The hosted MCP server at https://api.keploy.io/client/v1/mcp uses the same\n  kep_ PAT as a bearer token. The self-hosted Kubernetes Proxy REST API uses a\n  separate shared token (Authorization: Bearer <K8S_PROXY_SHARED_TOKEN>) per\n  https://keploy.io/docs/running-keploy/k8s-proxy-api/.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/keploy/refs/heads/main/authentication/keploy-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Testing & QA
- API Testing
- Integration/Regression Testing
- Unit Test Generation
- Contract Testing
- CI/CD
- Developer Tools
- AI / Agent Tooling
- eBPF / Observability
- Test Data & Mocking
---
