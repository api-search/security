---
api_key_in: []
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Funnel Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Funnel secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Funnel
provider_slug: funnel
scheme_count: 1
schemes:
- audience:
  - https://controlplane.setup.us.funnel.io
  - https://controlplane.setup.eu.funnel.io
  credentials:
  - client_id
  - client_secret
  description: Server-to-server OAuth 2.0 client-credentials flow. A "System user" is created per subscription in the Funnel app (Subscription overview -> Authentication), yielding a client_id and client_secret. These are exchanged at the Auth0 token endpoint with the region-appropriate audience for a Bearer access token used against the regional Control Plane API host.
  flow: clientCredentials
  grant_type: client_credentials
  identity_provider: Auth0
  name: FunnelSystemUserOAuth
  scopes: []
  sources:
  - registry.terraform.io/providers/funnel-io/funnel/latest/docs
  token_type: Bearer
  token_url: https://login.funnel.io/oauth/token
  token_url_eu: https://login.funnel.io/oauth/token
  type: oauth2
slug: funnel-authentication
source_filename: funnel-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: >-\n  https://registry.terraform.io/providers/funnel-io/funnel/latest/docs +\n  provider/auth/auth0_client.go (github.com/funnel-io/terraform-provider-funnel)\ndocs: https://registry.terraform.io/providers/funnel-io/funnel/latest/docs\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\n  api_key_in: []\nschemes:\n- name: FunnelSystemUserOAuth\n  type: oauth2\n  flow: clientCredentials\n  token_url: https://login.funnel.io/oauth/token\n  token_url_eu: https://login.funnel.io/oauth/token\n  identity_provider: Auth0\n  audience:\n  - https://controlplane.setup.us.funnel.io\n  - https://controlplane.setup.eu.funnel.io\n  grant_type: client_credentials\n  token_type: Bearer\n  credentials:\n  - client_id\n  - client_secret\n  scopes: []\n  sources:\n  - registry.terraform.io/providers/funnel-io/funnel/latest/docs\n  description: >-\n    Server-to-server OAuth 2.0 client-credentials flow. A \"System user\" is\
  \ created per subscription\n    in the Funnel app (Subscription overview -> Authentication), yielding a client_id and\n    client_secret. These are exchanged at the Auth0 token endpoint with the region-appropriate\n    audience for a Bearer access token used against the regional Control Plane API host.\nnotes: >-\n  No scope surface is documented (access is scoped by subscription and audience, not OAuth scopes),\n  so no scopes/ artifact is emitted. Authentication is region-aware: US and EU environments use\n  distinct audiences and Control Plane hosts (controlplane.setup.us|eu.funnel.io) for data residency.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/funnel/refs/heads/main/authentication/funnel-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Company
- Marketing
- Marketing Intelligence
- Marketing Data
- Analytics
- Advertising
- Data Integration
- ETL
- Data Warehouse
- Attribution
- Reporting
- Business Intelligence
---
