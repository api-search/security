---
api_key_in: []
api_specs:
- filename: DevTestLabs.json
  format: json
  label: Azure DevTest Labs API
  slug: azure-devtest-labs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/Azure/azure-rest-api-specs/main/specification/devtestlabs/resource-manager/Microsoft.DevTestLab/stable/2018-09-15/DevTestLabs.json
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Azure Test Labs Authentication
name_suffix: Authentication
oauth_flows:
- implicit
overview: Azure DevTest Labs secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the implicit flow(s).
provider_name: Azure DevTest Labs
provider_slug: azure-test-labs
scheme_count: 1
schemes:
- description: OAuth2 Implicit Grant
  flows:
  - authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize
    flow: implicit
    scopes: 1
  name: azure_auth
  sources:
  - openapi/azure-test-labs-openapi.yaml
  type: oauth2
slug: azure-test-labs-authentication
source_filename: azure-test-labs-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/azure-test-labs-openapi.yaml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - implicit\nschemes:\n- name: azure_auth\n  type: oauth2\n  flows:\n  - flow: implicit\n    authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize\n    scopes: 1\n  description: OAuth2 Implicit Grant\n  sources:\n  - openapi/azure-test-labs-openapi.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/azure-test-labs/refs/heads/main/authentication/azure-test-labs-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Azure
- Development
- Infrastructure
- Labs
- Testing
- Virtual Machines
---
