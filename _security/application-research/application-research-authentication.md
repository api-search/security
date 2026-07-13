---
api_key_in:
- header
api_specs:
- filename: score-openapi.yml
  format: yaml
  label: Score Workload Specification API
  slug: score-workload-specification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/application-research/refs/heads/main/openapi/score-openapi.yml
- filename: cloud-native-application-bundle-openapi.yml
  format: yaml
  label: Cloud Native Application Bundle API
  slug: cloud-native-application-bundle-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/application-research/refs/heads/main/openapi/cloud-native-application-bundle-openapi.yml
- filename: open-component-model-openapi.yml
  format: yaml
  label: Open Component Model API
  slug: open-component-model-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/application-research/refs/heads/main/openapi/open-component-model-openapi.yml
- filename: open-resource-discovery-openapi.yml
  format: yaml
  label: Open Resource Discovery API
  slug: open-resource-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/application-research/refs/heads/main/openapi/open-resource-discovery-openapi.yml
- filename: radius-openapi.yml
  format: yaml
  label: Radius Application Platform API
  slug: radius-application-platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/application-research/refs/heads/main/openapi/radius-openapi.yml
auth_types:
- apiKey
- http
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
method: derived
name: Application Research Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Application Research secures its APIs with apiKey, http, oauth2, and openIdConnect across 4 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Application Research
provider_slug: application-research
scheme_count: 4
schemes:
- bearerFormat: JWT
  description: JWT-based authentication
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/cloud-native-application-bundle-openapi.yml
  - openapi/open-component-model-openapi.yml
  - openapi/open-resource-discovery-openapi.yml
  - openapi/score-openapi.yml
  type: http
- description: API key authentication
  in: header
  name: apiKey
  parameter: X-API-Key
  sources:
  - openapi/cloud-native-application-bundle-openapi.yml
  - openapi/open-component-model-openapi.yml
  - openapi/score-openapi.yml
  type: apiKey
- description: OpenID Connect authentication
  name: oidc
  openIdConnectUrl: https://auth.ocm.example.com/.well-known/openid-configuration
  sources:
  - openapi/open-component-model-openapi.yml
  type: openIdConnect
- description: OAuth 2.0 authentication
  flows:
  - flow: clientCredentials
    scopes: 3
    tokenUrl: /oauth/token
  name: oauth2
  sources:
  - openapi/open-resource-discovery-openapi.yml
  type: oauth2
slug: application-research-authentication
source_filename: application-research-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/cloud-native-application-bundle-openapi.yml, openapi/open-component-model-openapi.yml,\n  openapi/open-resource-discovery-openapi.yml, openapi/score-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  - oauth2\n  - openIdConnect\n  api_key_in:\n  - header\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: JWT-based authentication\n  sources:\n  - openapi/cloud-native-application-bundle-openapi.yml\n  - openapi/open-component-model-openapi.yml\n  - openapi/open-resource-discovery-openapi.yml\n  - openapi/score-openapi.yml\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  description: API key authentication\n  sources:\n  - openapi/cloud-native-application-bundle-openapi.yml\n  - openapi/open-component-model-openapi.yml\n  - openapi/score-openapi.yml\n- name: oidc\n  type: openIdConnect\n  openIdConnectUrl:\
  \ https://auth.ocm.example.com/.well-known/openid-configuration\n  description: OpenID Connect authentication\n  sources:\n  - openapi/open-component-model-openapi.yml\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: /oauth/token\n    scopes: 3\n  description: OAuth 2.0 authentication\n  sources:\n  - openapi/open-resource-discovery-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/application-research/refs/heads/main/authentication/application-research-authentication.yml
summary_line: apiKey/http/oauth2/openIdConnect · 4 schemes
tags:
- Application Dependencies
- Cloud Native
- Integration
- Research
- Specifications
- Workload Specifications
---
