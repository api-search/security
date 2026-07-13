---
api_key_in: []
api_specs:
- filename: wso2-publisher-api.yaml
  format: yaml
  label: WSO2 Publisher API
  slug: publisher-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wso2/refs/heads/main/openapi/wso2-publisher-api.yaml
- filename: wso2-devportal-api.yaml
  format: yaml
  label: WSO2 Developer Portal API
  slug: devportal-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wso2/refs/heads/main/openapi/wso2-devportal-api.yaml
- filename: wso2-admin-api.yaml
  format: yaml
  label: WSO2 Admin Portal API
  slug: admin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wso2/refs/heads/main/openapi/wso2-admin-api.yaml
- filename: wso2-gateway-api.yaml
  format: yaml
  label: WSO2 Gateway API
  slug: gateway-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wso2/refs/heads/main/openapi/wso2-gateway-api.yaml
- filename: wso2-service-catalog-api.yaml
  format: yaml
  label: WSO2 Service Catalog API
  slug: service-catalog-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wso2/refs/heads/main/openapi/wso2-service-catalog-api.yaml
- filename: wso2-devops-api.yaml
  format: yaml
  label: WSO2 DevOps API
  slug: devops-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wso2/refs/heads/main/openapi/wso2-devops-api.yaml
- filename: wso2-dcr-api.yaml
  format: yaml
  label: WSO2 DCR API
  slug: dcr-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wso2/refs/heads/main/openapi/wso2-dcr-api.yaml
- filename: wso2-governance-api.yaml
  format: yaml
  label: WSO2 Governance API
  slug: governance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wso2/refs/heads/main/openapi/wso2-governance-api.yaml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Wso2 Authentication
name_suffix: Authentication
oauth_flows:
- password
overview: WSO2 secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the password flow(s).
provider_name: WSO2
provider_slug: wso2
scheme_count: 1
schemes:
- flows:
  - flow: password
    scopes: 41
    tokenUrl: https://localhost:9443/oauth2/token
  name: OAuth2Security
  sources:
  - openapi/wso2-admin-api.yaml
  - openapi/wso2-dcr-api.yaml
  - openapi/wso2-devportal-api.yaml
  - openapi/wso2-governance-api.yaml
  - openapi/wso2-service-catalog-api.yaml
  type: oauth2
slug: wso2-authentication
source_filename: wso2-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/wso2-admin-api.yaml, openapi/wso2-dcr-api.yaml, openapi/wso2-devportal-api.yaml,\n  openapi/wso2-governance-api.yaml, openapi/wso2-service-catalog-api.yaml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - password\nschemes:\n- name: OAuth2Security\n  type: oauth2\n  flows:\n  - flow: password\n    tokenUrl: https://localhost:9443/oauth2/token\n    scopes: 41\n  sources:\n  - openapi/wso2-admin-api.yaml\n  - openapi/wso2-dcr-api.yaml\n  - openapi/wso2-devportal-api.yaml\n  - openapi/wso2-governance-api.yaml\n  - openapi/wso2-service-catalog-api.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wso2/refs/heads/main/authentication/wso2-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- API Management
- Gateways
- Open Source
- API Lifecycle
- GraphQL
- SOAP
- REST
---
