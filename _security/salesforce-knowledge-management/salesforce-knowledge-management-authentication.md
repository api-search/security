---
api_key_in: []
api_specs:
- filename: salesforce-knowledge-management-rest-api-openapi.yml
  format: yaml
  label: Salesforce Knowledge REST API
  slug: salesforce-knowledge-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/salesforce-knowledge-management/refs/heads/main/openapi/salesforce-knowledge-management-rest-api-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Salesforce Knowledge Management Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Salesforce Knowledge Management secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Salesforce Knowledge Management
provider_slug: salesforce-knowledge-management
scheme_count: 2
schemes:
- flows:
  - authorizationUrl: https://login.salesforce.com/services/oauth2/authorize
    flow: authorizationCode
    scopes: 2
    tokenUrl: https://login.salesforce.com/services/oauth2/token
  name: oauth2
  sources:
  - openapi/salesforce-knowledge-management-rest-api-openapi.yml
  type: oauth2
- bearerFormat: JWT
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/salesforce-knowledge-management-rest-api-openapi.yml
  type: http
slug: salesforce-knowledge-management-authentication
source_filename: salesforce-knowledge-management-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/salesforce-knowledge-management-rest-api-openapi.yml\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://login.salesforce.com/services/oauth2/authorize\n    tokenUrl: https://login.salesforce.com/services/oauth2/token\n    scopes: 2\n  sources:\n  - openapi/salesforce-knowledge-management-rest-api-openapi.yml\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/salesforce-knowledge-management-rest-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/salesforce-knowledge-management/refs/heads/main/authentication/salesforce-knowledge-management-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Articles
- CRM
- Customer Service
- Documentation
- Knowledge Management
- Support
---
