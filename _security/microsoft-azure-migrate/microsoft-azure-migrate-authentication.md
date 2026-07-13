---
api_key_in: []
api_specs:
- filename: microsoft-azure-migrate-openapi.yml
  format: yaml
  label: Azure Migrate Projects API
  slug: azure-migrate-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-migrate/refs/heads/main/openapi/microsoft-azure-migrate-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Microsoft Azure Migrate Authentication
name_suffix: Authentication
oauth_flows:
- implicit
overview: Azure Migrate secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the implicit flow(s).
provider_name: Azure Migrate
provider_slug: microsoft-azure-migrate
scheme_count: 1
schemes:
- description: Azure Active Directory OAuth2 Flow.
  flows:
  - authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize
    flow: implicit
    scopes: 1
  name: azure_auth
  sources:
  - openapi/microsoft-azure-migrate-openapi.yml
  type: oauth2
slug: microsoft-azure-migrate-authentication
source_filename: microsoft-azure-migrate-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/microsoft-azure-migrate-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - implicit\nschemes:\n- name: azure_auth\n  type: oauth2\n  flows:\n  - flow: implicit\n    authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize\n    scopes: 1\n  description: Azure Active Directory OAuth2 Flow.\n  sources:\n  - openapi/microsoft-azure-migrate-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-migrate/refs/heads/main/authentication/microsoft-azure-migrate-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Assessment
- Cloud Migration
- Database Migration
- Discovery
- Migration
- Replication
- Server Migration
---
