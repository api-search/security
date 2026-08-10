---
api_key_in: []
api_specs:
- filename: nomad-health-default-api-openapi.yml
  format: yaml
  label: Nomad Health Default API
  slug: nomad-health-default-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nomad-health/refs/heads/main/openapi/nomad-health-default-api-openapi.yml
auth_types:
- session-cookie
description: ''
kind: authentication
layout: security
method: probed
name: Nomad Health Authentication
name_suffix: Authentication
oauth_flows: []
overview: Nomad Health secures its APIs with session-cookie across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Nomad Health
provider_slug: nomad-health
scheme_count: 1
schemes:
- description: 'Application session established through the browser sign-in flow at https://nomadhealth.com/sign-in. Requests without a valid session cookie receive HTTP 401 with the body {"code": "a0002", "error": "user is not authenticated"} on the /api/v1 surface and {"code": 401, "data": null, "message": null} on the /api surface. No bearer-token, API-key or OAuth alternative is offered publicly.'
  evidence:
  - body: '{"code": "a0002", "error": "user is not authenticated"}'
    http_status: 401
    url: https://nomadhealth.com/api/v1/accounts/me/
  - body: '{"code": "a0002", "error": "user is not authenticated"}'
    http_status: 401
    url: https://nomadhealth.com/api/v1/us/states/
  - body: '{"code": "a0002", "message": null, "data": null}'
    http_status: 401
    url: https://nomadhealth.com/api/emr_system
  in: cookie
  name: nomad-session
  sources:
  - openapi/nomad-health-platform-openapi.yml
  - openapi/nomad-health-api-openapi.yml
  type: session
slug: nomad-health-authentication
source_filename: nomad-health-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-04'\nmethod: probed\nsource: >-\n  live unauthenticated requests against https://nomadhealth.com/api/v1/* and\n  https://nomadhealth.com/api/*, plus the harvested Swagger 2.0 contracts\nnote: >-\n  Neither harvested Swagger document declares a securityDefinitions block, so nothing\n  could be derived mechanically (0-working/derive-authentication.py returned no profile).\n  Nomad Health publishes no developer authentication documentation and issues no public\n  API keys — this profile is written entirely from observed runtime behaviour.\nsummary:\n  types:\n  - session-cookie\n  api_key_in: []\n  oauth2_flows: []\n  public_credential_program: false\n  documented: false\nschemes:\n- name: nomad-session\n  type: session\n  in: cookie\n  description: >-\n    Application session established through the browser sign-in flow at\n    https://nomadhealth.com/sign-in. Requests without a valid session cookie receive\n    HTTP 401 with the body {\"code\": \"a0002\"\
  , \"error\": \"user is not authenticated\"} on\n    the /api/v1 surface and {\"code\": 401, \"data\": null, \"message\": null} on the /api\n    surface. No bearer-token, API-key or OAuth alternative is offered publicly.\n  sources:\n  - openapi/nomad-health-platform-openapi.yml\n  - openapi/nomad-health-api-openapi.yml\n  evidence:\n  - url: https://nomadhealth.com/api/v1/accounts/me/\n    http_status: 401\n    body: '{\"code\": \"a0002\", \"error\": \"user is not authenticated\"}'\n  - url: https://nomadhealth.com/api/v1/us/states/\n    http_status: 401\n    body: '{\"code\": \"a0002\", \"error\": \"user is not authenticated\"}'\n  - url: https://nomadhealth.com/api/emr_system\n    http_status: 401\n    body: '{\"code\": \"a0002\", \"message\": null, \"data\": null}'\nanonymous_operations:\n  note: >-\n    A small set of marketplace reference and job-search operations answer without any\n    credential. These are the only operations an unauthenticated client or agent can call.\n  operations:\n\
  \  - path: /api/v1/discipline-names/\n    method: get\n    http_status: 200\n  - path: /api/v1/jobposts/public_jobpost_search/\n    method: get\n    http_status: 200\n  - path: /api/v1/sitemap/jobs/chunk_count/\n    method: get\n    http_status: 200\n  - path: /api/v1/sitemap/jobs/chunk/\n    method: get\n    http_status: 200\n  - path: /api/region\n    method: get\n    http_status: 200\ngaps:\n  - No securityDefinitions in either published Swagger document, so the contract does not\n    state how to authenticate any of its 498 operations.\n  - No API key, personal access token or OAuth 2.0 authorization server is offered — an\n    integrator or agent has no first-class credential to obtain.\n  - No /.well-known/oauth-authorization-server or /.well-known/openid-configuration.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nomad-health/refs/heads/main/authentication/nomad-health-authentication.yml
summary_line: session-cookie · 1 scheme
tags:
- Company
- Healthcare
- Staffing
- Jobs
- Marketplace
- Travel Nursing
- Allied Health
- Credentialing
- Recruiting
- Human Resources
---
