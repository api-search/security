---
api_key_in: []
api_specs:
- filename: git.json
  format: json
  label: Azure DevOps Services REST API - Git
  slug: azure-devops-services-rest-api-git
  spec_type: OpenAPI
  url: https://github.com/MicrosoftDocs/vsts-rest-api-specs/blob/master/specification/git/7.1/git.json
- filename: tfvc.json
  format: json
  label: Azure DevOps Services REST API - TFVC
  slug: azure-devops-services-rest-api-tfvc
  spec_type: OpenAPI
  url: https://github.com/MicrosoftDocs/vsts-rest-api-specs/blob/master/specification/tfvc/7.1/tfvc.json
- filename: policy.json
  format: json
  label: Azure DevOps Services REST API - Policy
  slug: azure-devops-services-rest-api-policy
  spec_type: OpenAPI
  url: https://github.com/MicrosoftDocs/vsts-rest-api-specs/blob/master/specification/policy/7.1/policy.json
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Microsoft Azure Repo Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Azure Repos secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Azure Repos
provider_slug: microsoft-azure-repo
scheme_count: 2
schemes:
- description: OAuth 2.0 authorization code flow for Azure DevOps Services. Requires the vso.code scope for read operations and vso.code_write for write operations.
  flows:
  - authorizationUrl: https://app.vssps.visualstudio.com/oauth2/authorize
    flow: authorizationCode
    scopes: 3
    tokenUrl: https://app.vssps.visualstudio.com/oauth2/token
  name: oauth2
  sources:
  - openapi/azure-repo-git-api-openapi.yml
  type: oauth2
- description: HTTP Basic authentication using a Personal Access Token (PAT). Use any string for the username and the PAT as the password.
  name: basicAuth
  scheme: basic
  sources:
  - openapi/azure-repo-git-api-openapi.yml
  type: http
slug: microsoft-azure-repo-authentication
source_filename: microsoft-azure-repo-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/azure-repo-git-api-openapi.yml\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://app.vssps.visualstudio.com/oauth2/authorize\n    tokenUrl: https://app.vssps.visualstudio.com/oauth2/token\n    scopes: 3\n  description: OAuth 2.0 authorization code flow for Azure DevOps Services. Requires the vso.code\n    scope for read operations and vso.code_write for write operations.\n  sources:\n  - openapi/azure-repo-git-api-openapi.yml\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: HTTP Basic authentication using a Personal Access Token (PAT). Use any string\n    for the username and the PAT as the password.\n  sources:\n  - openapi/azure-repo-git-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-repo/refs/heads/main/authentication/microsoft-azure-repo-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- DevOps
- Git
- Repositories
- Source Control
- TFVC
- Version Control
---
