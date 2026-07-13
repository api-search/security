---
api_key_in: []
api_specs:
- filename: azure-devops-work-items-openapi.yml
  format: yaml
  label: Azure DevOps Work Item Tracking API
  slug: azure-devops-work-item-tracking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/azure-devops/refs/heads/main/openapi/azure-devops-work-items-openapi.yml
- filename: azure-devops-pipelines-openapi.yml
  format: yaml
  label: Azure DevOps Pipelines API
  slug: azure-devops-pipelines-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/azure-devops/refs/heads/main/openapi/azure-devops-pipelines-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Azure Devops Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Azure DevOps secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Azure DevOps
provider_slug: azure-devops
scheme_count: 2
schemes:
- name: personalAccessToken
  scheme: basic
  sources:
  - openapi/azure-devops-pipelines-openapi.yml
  - openapi/azure-devops-work-items-openapi.yml
  type: http
- flows:
  - authorizationUrl: https://app.vssps.visualstudio.com/oauth2/authorize
    flow: authorizationCode
    scopes: 2
    tokenUrl: https://app.vssps.visualstudio.com/oauth2/token
  name: oauth2
  sources:
  - openapi/azure-devops-pipelines-openapi.yml
  - openapi/azure-devops-work-items-openapi.yml
  type: oauth2
slug: azure-devops-authentication
source_filename: azure-devops-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/azure-devops-pipelines-openapi.yml, openapi/azure-devops-work-items-openapi.yml\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: personalAccessToken\n  type: http\n  scheme: basic\n  sources:\n  - openapi/azure-devops-pipelines-openapi.yml\n  - openapi/azure-devops-work-items-openapi.yml\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://app.vssps.visualstudio.com/oauth2/authorize\n    tokenUrl: https://app.vssps.visualstudio.com/oauth2/token\n    scopes: 2\n  sources:\n  - openapi/azure-devops-pipelines-openapi.yml\n  - openapi/azure-devops-work-items-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/azure-devops/refs/heads/main/authentication/azure-devops-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Azure
- CI/CD
- DevOps
- Pipelines
- Work Items
---
