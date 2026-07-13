---
api_key_in: []
api_specs:
- filename: ariba-sourcing-external-approval-api.yaml
  format: yaml
  label: Ariba Sourcing - External Approval API
  slug: ariba-sourcing-external-approval-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ariba-sourcing/refs/heads/main/openapi/ariba-sourcing-external-approval-api.yaml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Ariba Sourcing Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Ariba Sourcing secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Ariba Sourcing
provider_slug: ariba-sourcing
scheme_count: 1
schemes:
- description: OAuth 2.0 authentication. Obtain access token from https://api.ariba.com/v2/oauth/token using client credentials.
  flows:
  - flow: clientCredentials
    scopes: 0
    tokenUrl: https://api.ariba.com/v2/oauth/token
  name: OAuth2
  sources:
  - openapi/ariba-sourcing-external-approval-api.yaml
  type: oauth2
slug: ariba-sourcing-authentication
source_filename: ariba-sourcing-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/ariba-sourcing-external-approval-api.yaml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.ariba.com/v2/oauth/token\n    scopes: 0\n  description: OAuth 2.0 authentication. Obtain access token from https://api.ariba.com/v2/oauth/token\n    using client credentials.\n  sources:\n  - openapi/ariba-sourcing-external-approval-api.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ariba-sourcing/refs/heads/main/authentication/ariba-sourcing-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Approvals
- Auctions
- B2B
- Contracts
- Procurement
- RFx
- SAP
- Sourcing
- Supplier Management
- Supply Chain
---
