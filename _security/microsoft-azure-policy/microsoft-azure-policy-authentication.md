---
anonymous_access: false
api_key_in: []
api_specs:
- filename: microsoft-azure-policy-operations-api-openapi.yml
  format: yaml
  label: Azure Policy Operations API
  slug: microsoft-azure-policy-operations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-azure-policy/openapi/microsoft-azure-policy-operations-api-openapi.yml
- filename: policyDefinitions.json
  format: json
  label: Azure Policy REST API
  slug: microsoft-azure-policy-policy-definitions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/Azure/azure-rest-api-specs/main/specification/resources/resource-manager/Microsoft.Authorization/policy/stable/2025-01-01/policyDefinitions.json
- filename: microsoft-azure-policy-policyassignments-api-openapi.yml
  format: yaml
  label: Azure Policy Policy Assignments API
  slug: microsoft-azure-policy-policyassignments-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-azure-policy/openapi/microsoft-azure-policy-policyassignments-api-openapi.yml
- filename: microsoft-azure-policy-policydefinitions-api-openapi.yml
  format: yaml
  label: Azure Policy Policy Definitions API
  slug: microsoft-azure-policy-policydefinitions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-azure-policy/openapi/microsoft-azure-policy-policydefinitions-api-openapi.yml
- filename: microsoft-azure-policy-policydefinitionversions-api-openapi.yml
  format: yaml
  label: Azure Policy Policy Definition Versions API
  slug: microsoft-azure-policy-policydefinitionversions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-azure-policy/openapi/microsoft-azure-policy-policydefinitionversions-api-openapi.yml
- filename: microsoft-azure-policy-policysetdefinitions-api-openapi.yml
  format: yaml
  label: Azure Policy Policy Set Definitions API
  slug: microsoft-azure-policy-policysetdefinitions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-azure-policy/openapi/microsoft-azure-policy-policysetdefinitions-api-openapi.yml
- filename: microsoft-azure-policy-policysetdefinitionversions-api-openapi.yml
  format: yaml
  label: Azure Policy Policy Set Definition Versions API
  slug: microsoft-azure-policy-policysetdefinitionversions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-azure-policy/openapi/microsoft-azure-policy-policysetdefinitionversions-api-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Microsoft Azure Policy Authentication
name_suffix: Authentication
oauth_flows:
- implicit
overview: Azure Policy secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the implicit flow(s).
provider_name: Azure Policy
provider_slug: microsoft-azure-policy
scheme_count: 1
schemes:
- description: Azure Active Directory OAuth2 Flow.
  flows:
  - authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize
    flow: implicit
    scopes: 1
  name: azure_auth
  sources:
  - openapi/microsoft-azure-policy-openapi.yml
  - openapi/microsoft-azure-policy-operations-api-openapi.yml
  - openapi/microsoft-azure-policy-policy-definitions-api-openapi.yml
  type: oauth2
slug: microsoft-azure-policy-authentication
source_filename: microsoft-azure-policy-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: derived\nsource: openapi/microsoft-azure-policy-openapi.yml, openapi/microsoft-azure-policy-operations-api-openapi.yml,\n  openapi/microsoft-azure-policy-policy-definitions-api-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - implicit\nschemes:\n- name: azure_auth\n  type: oauth2\n  flows:\n  - flow: implicit\n    authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize\n    scopes: 1\n  description: Azure Active Directory OAuth2 Flow.\n  sources:\n  - openapi/microsoft-azure-policy-openapi.yml\n  - openapi/microsoft-azure-policy-operations-api-openapi.yml\n  - openapi/microsoft-azure-policy-policy-definitions-api-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/microsoft-azure-policy/authentication/microsoft-azure-policy-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Compliance
- Governance
- Policy
- Resource Management
---
