---
api_key_in: []
api_specs:
- filename: microsoft-azure-integration-services-openapi.yml
  format: yaml
  label: Azure API Management
  slug: azure-api-management
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-integration-services/refs/heads/main/openapi/microsoft-azure-integration-services-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Microsoft Azure Integration Services Authentication
name_suffix: Authentication
oauth_flows:
- implicit
overview: Microsoft Azure Integration Services secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the implicit flow(s).
provider_name: Microsoft Azure Integration Services
provider_slug: microsoft-azure-integration-services
scheme_count: 1
schemes:
- description: Azure Active Directory OAuth2 Flow.
  flows:
  - authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize
    flow: implicit
    scopes: 1
  name: azure_auth
  sources:
  - openapi/microsoft-azure-integration-services-openapi.yml
  type: oauth2
slug: microsoft-azure-integration-services-authentication
source_filename: microsoft-azure-integration-services-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/microsoft-azure-integration-services-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - implicit\nschemes:\n- name: azure_auth\n  type: oauth2\n  flows:\n  - flow: implicit\n    authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize\n    scopes: 1\n  description: Azure Active Directory OAuth2 Flow.\n  sources:\n  - openapi/microsoft-azure-integration-services-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-integration-services/refs/heads/main/authentication/microsoft-azure-integration-services-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- API Management
- Enterprise
- Event-Driven
- Integration
- Messaging
---
