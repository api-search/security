---
api_key_in: []
api_specs:
- filename: spinnaker-applications-api-openapi.yml
  format: yaml
  label: Spinnaker Applications API
  slug: spinnaker-applications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spinnaker/refs/heads/main/openapi/spinnaker-applications-api-openapi.yml
- filename: spinnaker-build-services-api-openapi.yml
  format: yaml
  label: Spinnaker Build Services API
  slug: spinnaker-build-services-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spinnaker/refs/heads/main/openapi/spinnaker-build-services-api-openapi.yml
- filename: spinnaker-clusters-api-openapi.yml
  format: yaml
  label: Spinnaker Clusters API
  slug: spinnaker-clusters-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spinnaker/refs/heads/main/openapi/spinnaker-clusters-api-openapi.yml
- filename: spinnaker-images-api-openapi.yml
  format: yaml
  label: Spinnaker Images API
  slug: spinnaker-images-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spinnaker/refs/heads/main/openapi/spinnaker-images-api-openapi.yml
- filename: spinnaker-load-balancers-api-openapi.yml
  format: yaml
  label: Spinnaker Load Balancers API
  slug: spinnaker-load-balancers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spinnaker/refs/heads/main/openapi/spinnaker-load-balancers-api-openapi.yml
- filename: spinnaker-pipelines-api-openapi.yml
  format: yaml
  label: Spinnaker Pipelines API
  slug: spinnaker-pipelines-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spinnaker/refs/heads/main/openapi/spinnaker-pipelines-api-openapi.yml
- filename: spinnaker-projects-api-openapi.yml
  format: yaml
  label: Spinnaker Projects API
  slug: spinnaker-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spinnaker/refs/heads/main/openapi/spinnaker-projects-api-openapi.yml
- filename: spinnaker-search-api-openapi.yml
  format: yaml
  label: Spinnaker Search API
  slug: spinnaker-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spinnaker/refs/heads/main/openapi/spinnaker-search-api-openapi.yml
- filename: spinnaker-tasks-api-openapi.yml
  format: yaml
  label: Spinnaker Tasks API
  slug: spinnaker-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spinnaker/refs/heads/main/openapi/spinnaker-tasks-api-openapi.yml
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
