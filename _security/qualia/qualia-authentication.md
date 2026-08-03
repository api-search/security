---
api_key_in: []
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Qualia Authentication
name_suffix: Authentication
oauth_flows: []
overview: Qualia secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Qualia
provider_slug: qualia
scheme_count: 1
schemes:
- description: Users are authenticated via a basic HTTP authentication framework to identify the organization calling Qualia. Credentials are issued per organization by Qualia; there is no public self-service key provisioning.
  in: header
  name: basicAuth
  parameter: Authorization
  scheme: basic
  sources:
  - https://www.qualia.com/qualia-api/
  - probe:https://api.qualia.com/graphql
  type: http
slug: qualia-authentication
source_filename: qualia-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-02'\nmethod: searched\nsource: https://www.qualia.com/qualia-api/\ndocs: https://www.qualia.com/qualia-api/\nnote: 'Derived from the provider''s published API documentation plus a live unauthenticated\n  probe of the GraphQL endpoint. Qualia publishes no OpenAPI, so no securityScheme\n  block could be derived mechanically.'\nsummary:\n  types:\n  - http\n  http_schemes:\n  - basic\n  api_key_in: []\n  oauth2_flows: []\n  authorization_model: capability-gates\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: 'Users are authenticated via a basic HTTP authentication framework to\n    identify the organization calling Qualia. Credentials are issued per organization\n    by Qualia; there is no public self-service key provisioning.'\n  in: header\n  parameter: Authorization\n  sources:\n  - https://www.qualia.com/qualia-api/\n  - probe:https://api.qualia.com/graphql\nauthorization:\n  model: capability-gates\n  description: 'Beyond authentication,\
  \ the Qualia API gates every call behind capability\n    gates — grants organized around an objective (placing orders, messaging, documents,\n    reporting) that Qualia enables on a per-organization basis. Granular controls grant\n    or revoke API access to owned or partner organizations to retrieve data on behalf\n    of the end consumer, so a valid credential does not imply access to every operation.'\n  provisioning: Contact Qualia to have capability gates enabled on your organization.\n  docs: https://www.qualia.com/qualia-api/\noauth:\n  supported: false\n  evidence: '/.well-known/openid-configuration and /.well-known/oauth-authorization-server\n    both return 404 on www.qualia.com; the docs describe HTTP Basic only.'\nobserved:\n  unauthenticated_response:\n    http_status: 401\n    body: '{\"errors\":[{\"message\":\"Authorization header is missing\",\"extensions\":{\"code\":\"UNAUTHORIZED\"}}]}'\n    probed: '2026-08-02'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/qualia/refs/heads/main/authentication/qualia-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Real Estate
- Title Insurance
- Escrow
- Mortgage
- Closing
- Settlement Services
- PropTech
- Financial Services
- GraphQL
---
