---
anonymous_access: false
api_key_in: []
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Qualia Title Authentication
name_suffix: Authentication
oauth_flows: []
overview: Qualia secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Qualia
provider_slug: qualia-title
scheme_count: 1
schemes:
- header: Authorization
  identifies: calling organization
  in: header
  name: basicAuth
  scheme: basic
  sources:
  - https://www.qualia.com/qualia-api/
  type: http
slug: qualia-title-authentication
source_filename: qualia-title-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-16'\nmethod: searched\nsource: https://www.qualia.com/qualia-api/\ndocs: https://www.qualia.com/qualia-api/\nprovider: Qualia\nproviderId: qualia-title\nnote: >-\n  No OpenAPI or public GraphQL schema exists to derive security schemes from\n  (derive-authentication.py found none). This profile is taken from Qualia's\n  public API page, which states \"Users are authenticated via a basic HTTP\n  authentication framework to identify the organization calling Qualia\", and is\n  corroborated by anonymous probes of the live endpoint recorded under\n  x-evidence. Credentials are issued per organization through Qualia's gated\n  onboarding; no credential format or sandbox key prefix is published.\nsummary:\n  types:\n  - http\n  http_schemes:\n  - basic\n  api_key_in: []\n  oauth2_flows: []\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  in: header\n  header: Authorization\n  identifies: calling organization\n  sources:\n  - https://www.qualia.com/qualia-api/\n\
  authorization:\n  model: capability gates + authorized organizations\n  capability_gates: >-\n    The Qualia API is organized by capability gates, which provide access to\n    calls around an objective; customers purchase the capabilities they need.\n  authorized_organizations: >-\n    Granular controls to grant (or revoke) API access to owned or partner\n    organizations to retrieve data on behalf of the end consumer.\n  source: https://www.qualia.com/qualia-api/\noauth2: false\nopenid_connect: false\nscopes: none published (access is scoped by capability gates, not OAuth scopes)\nx-evidence:\n  endpoint: https://api.qualia.com/graphql\n  fetched: '2026-09-16'\n  probes:\n  - request: POST without Authorization header\n    http_status: 401\n    body: '{\"errors\":[{\"message\":\"Authorization header is missing\",\"extensions\":{\"code\":\"UNAUTHORIZED\"}}]}'\n  - request: POST with Authorization Bearer <token>\n    http_status: 401\n    body: '{\"errors\":[{\"message\":\"Authorization\
  \ header is not properly formatted\",\"extensions\":{\"code\":\"UNAUTHORIZED\"}}]}'\n  - request: POST with Authorization Basic <invalid credentials>\n    http_status: 403\n    body: '{\"errors\":[{\"message\":\"User is not authenticated\",\"extensions\":{\"code\":\"FORBIDDEN\"}}]}'\n  interpretation: >-\n    A Bearer header is rejected as malformed while a Basic header is parsed and\n    then rejected on credentials, confirming HTTP Basic is the accepted scheme.\n  well_known:\n  - url: https://api.qualia.com/.well-known/oauth-authorization-server\n    http_status: 404\n  - url: https://api.qualia.com/.well-known/oauth-protected-resource\n    http_status: 404\n  - url: https://api.qualia.com/.well-known/openid-configuration\n    http_status: 404\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/qualia-title/refs/heads/main/authentication/qualia-title-authentication.yml
summary_line: http · 1 scheme
tags:
- Title Insurance
- Escrow
- Real-Estate
- Closing
- Settlement
- PropTech
- GraphQL
---
