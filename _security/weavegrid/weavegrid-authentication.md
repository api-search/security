---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: probed
name: Weavegrid Authentication
name_suffix: Authentication
oauth_flows: []
overview: WeaveGrid declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: WeaveGrid
provider_slug: weavegrid
scheme_count: 1
schemes:
- description: 'The only authentication mechanism observable without credentials. The API host answers protected routes with HTTP 401 and the response header "WWW-Authenticate: Basic", which instructs a client to retry with an Authorization: Basic credential. Whether Basic guards the whole API or only the documentation routes cannot be determined anonymously.'
  header: Authorization
  id: http_basic
  in: header
  observed:
    body: '{"detail":"Not authenticated"}'
    content_type: application/json
    date: '2026-09-04'
    status: 401
    url: https://api.weavegrid.com/openapi.json
    www_authenticate: Basic
  scheme: basic
  type: http
slug: weavegrid-authentication
source_filename: weavegrid-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-04'\nmethod: probed\nsource: https://api.weavegrid.com/openapi.json\nnote: >-\n  This profile is PROBED from the live authentication challenge returned by WeaveGrid's production API\n  host, not read from provider documentation. WeaveGrid publishes no public authentication page, no\n  developer portal and no reference, so no `Authentication` pointer is wired into apis.yml `common[]`:\n  that check credits a provider for DOCUMENTING authentication, and WeaveGrid does not. The pointer is\n  attached to the API entry as a description of what we observed, which is a different claim.\napi: weavegrid-partner-api\nhost: api.weavegrid.com\nserver_stack:\n  framework: FastAPI\n  server_header: uvicorn\n  evidence: >-\n    /openapi.json and /docs both exist and challenge, while every other path returns the FastAPI\n    default body {\"detail\":\"Not Found\"} — the signature of a FastAPI app with its auto-generated\n    OpenAPI document and Swagger UI mounted at the\
  \ default locations and placed behind a dependency.\n  first_party_evidence: >-\n    Responses carry an \"x-wg-log-session\" header on WeaveGrid's own registrable domain, and CAA/SPF\n    records for weavegrid.com cover the host, so the surface belongs to WeaveGrid.\nschemes:\n- id: http_basic\n  type: http\n  scheme: basic\n  in: header\n  header: Authorization\n  description: >-\n    The only authentication mechanism observable without credentials. The API host answers protected\n    routes with HTTP 401 and the response header \"WWW-Authenticate: Basic\", which instructs a client to\n    retry with an Authorization: Basic credential. Whether Basic guards the whole API or only the\n    documentation routes cannot be determined anonymously.\n  observed:\n    url: https://api.weavegrid.com/openapi.json\n    status: 401\n    www_authenticate: Basic\n    body: '{\"detail\":\"Not authenticated\"}'\n    content_type: application/json\n    date: '2026-09-04'\noauth2: false\nopenid_connect:\
  \ false\napi_key: false\nmutual_tls: false\ncredential_acquisition:\n  self_serve: false\n  route: >-\n    No public sign-up for API access. WeaveGrid's partners page invites aggregators to \"Plug into our\n    partner API\" and routes them to a \"Become a partner\" contact form; credentials are issued through\n    that commercial conversation.\n  url: https://www.weavegrid.com/partners\n  status: 200\ngaps:\n- No public authentication documentation page.\n- No token endpoint, OAuth metadata or OpenID discovery document on any WeaveGrid host.\n- Scope model unknown; no OAuth surface exists, so scopes/ is correctly absent rather than empty.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/weavegrid/refs/heads/main/authentication/weavegrid-authentication.yml
summary_line: 1 scheme
tags:
- Energy
- Electric Utilities
- Electric Vehicles
- EV Charging
- Smart Grid
- Managed Charging
- Distributed Energy Resources
- Demand Response
- Grid Orchestration
- Vehicle Telematics
- Climate Tech
- Company
---
