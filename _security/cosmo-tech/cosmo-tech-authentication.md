---
api_key_in: []
api_specs:
- filename: cosmo-tech-organization-openapi-original.yaml
  format: yaml
  label: Cosmo Tech Cloud Platform API
  slug: cosmo-tech-cloud-platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cosmo-tech/refs/heads/main/openapi/cosmo-tech-organization-openapi-original.yaml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Cosmo Tech Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Cosmo Tech secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Cosmo Tech
provider_slug: cosmo-tech
scheme_count: 1
schemes:
- description: OAuth2 authentication
  flows:
  - authorizationUrl: https://example.com/authorize
    flow: authorizationCode
    scopes: 0
    tokenUrl: https://example.com/token
  name: oAuth2AuthCode
  sources:
  - openapi/cosmo-tech-dataset-openapi-original.yaml
  - openapi/cosmo-tech-meta-openapi-original.yaml
  - openapi/cosmo-tech-organization-openapi-original.yaml
  - openapi/cosmo-tech-run-openapi-original.yaml
  - openapi/cosmo-tech-runner-openapi-original.yaml
  - openapi/cosmo-tech-solution-openapi-original.yaml
  - openapi/cosmo-tech-workspace-openapi-original.yaml
  type: oauth2
slug: cosmo-tech-authentication
source_filename: cosmo-tech-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: derived\nsource: openapi/cosmo-tech-dataset-openapi-original.yaml, openapi/cosmo-tech-meta-openapi-original.yaml,\n  openapi/cosmo-tech-organization-openapi-original.yaml, openapi/cosmo-tech-run-openapi-original.yaml,\n  openapi/cosmo-tech-runner-openapi-original.yaml, openapi/cosmo-tech-solution-openapi-original.yaml,\n  openapi/cosmo-tech-workspace-openapi-original.yaml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: oAuth2AuthCode\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://example.com/authorize\n    tokenUrl: https://example.com/token\n    scopes: 0\n  description: OAuth2 authentication\n  sources:\n  - openapi/cosmo-tech-dataset-openapi-original.yaml\n  - openapi/cosmo-tech-meta-openapi-original.yaml\n  - openapi/cosmo-tech-organization-openapi-original.yaml\n  - openapi/cosmo-tech-run-openapi-original.yaml\n  - openapi/cosmo-tech-runner-openapi-original.yaml\n\
  \  - openapi/cosmo-tech-solution-openapi-original.yaml\n  - openapi/cosmo-tech-workspace-openapi-original.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cosmo-tech/refs/heads/main/authentication/cosmo-tech-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Company
- Simulation
- Digital Twin
- Artificial Intelligence
- Supply Chain
- Predictive Analytics
- Industrial
---
