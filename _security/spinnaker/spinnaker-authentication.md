---
api_key_in: []
api_specs:
- filename: spinnaker-gate-openapi.yml
  format: yaml
  label: Spinnaker Gate API
  slug: spinnaker-gate-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spinnaker/refs/heads/main/openapi/spinnaker-gate-openapi.yml
auth_types:
- mutualTLS
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Spinnaker Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Spinnaker secures its APIs with mutualTLS and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Spinnaker
provider_slug: spinnaker
scheme_count: 2
schemes:
- description: OAuth 2.0 authentication for Spinnaker Gate
  flows:
  - authorizationUrl: https://accounts.example.com/oauth/authorize
    flow: authorizationCode
    scopes: 3
    tokenUrl: https://accounts.example.com/oauth/token
  name: oauth2
  sources:
  - openapi/spinnaker-gate-openapi.yml
  type: oauth2
- description: X.509 certificate-based mutual TLS authentication
  name: x509
  sources:
  - openapi/spinnaker-gate-openapi.yml
  type: mutualTLS
slug: spinnaker-authentication
source_filename: spinnaker-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/spinnaker-gate-openapi.yml\nsummary:\n  types:\n  - mutualTLS\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://accounts.example.com/oauth/authorize\n    tokenUrl: https://accounts.example.com/oauth/token\n    scopes: 3\n  description: OAuth 2.0 authentication for Spinnaker Gate\n  sources:\n  - openapi/spinnaker-gate-openapi.yml\n- name: x509\n  type: mutualTLS\n  description: X.509 certificate-based mutual TLS authentication\n  sources:\n  - openapi/spinnaker-gate-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/spinnaker/refs/heads/main/authentication/spinnaker-authentication.yml
summary_line: mutualTLS/oauth2 · 2 schemes
tags:
- Continuous Delivery
- Containers
- DevOps
- Multi-Cloud
- Pipelines
---
