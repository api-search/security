---
api_key_in:
- header
api_specs:
- filename: overview
  format: yaml
  label: Microsoft Graph API
  slug: microsoft-graph-api
  spec_type: OpenAPI
  url: https://learn.microsoft.com/en-us/graph/api/overview
- filename: microsoft-azure-rest-openapi.yml
  format: yaml
  label: Azure REST API
  slug: azure-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft/refs/heads/main/openapi/microsoft-azure-rest-openapi.yml
- filename: microsoft-azure-openai-openapi.yml
  format: yaml
  label: Azure OpenAI Service API
  slug: azure-openai-service-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft/refs/heads/main/openapi/microsoft-azure-openai-openapi.yml
- filename: microsoft-azure-cognitive-services-openapi.yml
  format: yaml
  label: Azure Cognitive Services API
  slug: azure-cognitive-services-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft/refs/heads/main/openapi/microsoft-azure-cognitive-services-openapi.yml
- filename: microsoft-teams-openapi.yml
  format: yaml
  label: Microsoft Teams API
  slug: microsoft-teams-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft/refs/heads/main/openapi/microsoft-teams-openapi.yml
- filename: microsoft-onedrive-openapi.yml
  format: yaml
  label: OneDrive API
  slug: onedrive-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft/refs/heads/main/openapi/microsoft-onedrive-openapi.yml
- filename: microsoft-power-platform-openapi.yml
  format: yaml
  label: Power Platform API
  slug: power-platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft/refs/heads/main/openapi/microsoft-power-platform-openapi.yml
- filename: microsoft-bing-search-openapi.yml
  format: yaml
  label: Bing Search APIs
  slug: bing-search-apis
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft/refs/heads/main/openapi/microsoft-bing-search-openapi.yml
- filename: microsoft-sharepoint-openapi.yml
  format: yaml
  label: SharePoint REST API
  slug: sharepoint-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft/refs/heads/main/openapi/microsoft-sharepoint-openapi.yml
- filename: microsoft-power-bi-openapi.yml
  format: yaml
  label: Power BI REST API
  slug: power-bi-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft/refs/heads/main/openapi/microsoft-power-bi-openapi.yml
- filename: microsoft-azure-devops-openapi.yml
  format: yaml
  label: Azure DevOps REST API
  slug: azure-devops-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft/refs/heads/main/openapi/microsoft-azure-devops-openapi.yml
- filename: microsoft-dynamics-365-openapi.yml
  format: yaml
  label: Dynamics 365 REST API
  slug: dynamics-365-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft/refs/heads/main/openapi/microsoft-dynamics-365-openapi.yml
- filename: microsoft-linkedin-openapi.yml
  format: yaml
  label: LinkedIn API
  slug: linkedin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft/refs/heads/main/openapi/microsoft-linkedin-openapi.yml
- filename: microsoft-azure-communication-services-openapi.yml
  format: yaml
  label: Azure Communication Services API
  slug: azure-communication-services-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft/refs/heads/main/openapi/microsoft-azure-communication-services-openapi.yml
- filename: microsoft-entra-id-openapi.yml
  format: yaml
  label: Microsoft Entra ID API
  slug: microsoft-entra-id-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft/refs/heads/main/openapi/microsoft-entra-id-openapi.yml
- filename: microsoft-outlook-openapi.yml
  format: yaml
  label: Microsoft Outlook API
  slug: microsoft-outlook-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft/refs/heads/main/openapi/microsoft-outlook-openapi.yml
- filename: microsoft-intune-openapi.yml
  format: yaml
  label: Microsoft Intune API
  slug: microsoft-intune-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft/refs/heads/main/openapi/microsoft-intune-openapi.yml
auth_types:
- apiKey
- http
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Microsoft Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
overview: Microsoft secures its APIs with apiKey, http, and oauth2 across 7 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and clientCredentials flow(s).
provider_name: Microsoft
provider_slug: microsoft
scheme_count: 7
schemes:
- description: Azure Cognitive Services subscription key
  in: header
  name: apiKey
  parameter: Ocp-Apim-Subscription-Key
  sources:
  - openapi/microsoft-azure-cognitive-services-openapi.yml
  - openapi/microsoft-bing-search-openapi.yml
  type: apiKey
- description: HMAC-SHA256 signature authentication
  in: header
  name: accessKey
  parameter: Authorization
  sources:
  - openapi/microsoft-azure-communication-services-openapi.yml
  type: apiKey
- description: Personal Access Token (PAT) as password with empty username
  name: basicAuth
  scheme: basic
  sources:
  - openapi/microsoft-azure-devops-openapi.yml
  type: http
- description: Microsoft Entra ID OAuth 2.0
  flows:
  - authorizationUrl: https://app.vssps.visualstudio.com/oauth2/authorize
    flow: authorizationCode
    scopes: 4
    tokenUrl: https://app.vssps.visualstudio.com/oauth2/token
  name: oauth2
  sources:
  - openapi/microsoft-azure-devops-openapi.yml
  - openapi/microsoft-dynamics-365-openapi.yml
  - openapi/microsoft-onedrive-openapi.yml
  - openapi/microsoft-outlook-openapi.yml
  - openapi/microsoft-power-bi-openapi.yml
  - openapi/microsoft-power-platform-openapi.yml
  - openapi/microsoft-sharepoint-openapi.yml
  - openapi/microsoft-teams-openapi.yml
  type: oauth2
- description: Azure OpenAI API key
  in: header
  name: apiKey
  parameter: api-key
  sources:
  - openapi/microsoft-azure-openai-openapi.yml
  type: apiKey
- description: Microsoft Entra ID OAuth 2.0
  flows:
  - flow: clientCredentials
    scopes: 1
    tokenUrl: https://login.microsoftonline.com/{tenantId}/oauth2/v2.0/token
  name: oauth2
  sources:
  - openapi/microsoft-azure-openai-openapi.yml
  - openapi/microsoft-azure-rest-openapi.yml
  - openapi/microsoft-entra-id-openapi.yml
  - openapi/microsoft-intune-openapi.yml
  type: oauth2
- description: Microsoft identity platform OAuth 2.0 authorization
  flows:
  - authorizationUrl: https://login.microsoftonline.com/common/oauth2/v2.0/authorize
    flow: authorizationCode
    scopes: 20
    tokenUrl: https://login.microsoftonline.com/common/oauth2/v2.0/token
  - flow: clientCredentials
    scopes: 1
    tokenUrl: https://login.microsoftonline.com/{tenant}/oauth2/v2.0/token
  name: oauth2
  sources:
  - openapi/microsoft-graph-openapi.yml
  type: oauth2
slug: microsoft-authentication
source_filename: microsoft-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/microsoft-azure-cognitive-services-openapi.yml, openapi/microsoft-azure-communication-services-openapi.yml,\n  openapi/microsoft-azure-devops-openapi.yml, openapi/microsoft-azure-openai-openapi.yml, openapi/microsoft-azure-rest-openapi.yml,\n  openapi/microsoft-bing-search-openapi.yml, openapi/microsoft-dynamics-365-openapi.yml, openapi/microsoft-entra-id-openapi.yml,\n  openapi/microsoft-graph-openapi.yml, openapi/microsoft-intune-openapi.yml, openapi/microsoft-onedrive-openapi.yml,\n  openapi/microsoft-outlook-openapi.yml ...\nsummary:\n  types:\n  - apiKey\n  - http\n  - oauth2\n  api_key_in:\n  - header\n  oauth2_flows:\n  - authorizationCode\n  - clientCredentials\nschemes:\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: Ocp-Apim-Subscription-Key\n  description: Azure Cognitive Services subscription key\n  sources:\n  - openapi/microsoft-azure-cognitive-services-openapi.yml\n  - openapi/microsoft-bing-search-openapi.yml\n\
  - name: accessKey\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: HMAC-SHA256 signature authentication\n  sources:\n  - openapi/microsoft-azure-communication-services-openapi.yml\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: Personal Access Token (PAT) as password with empty username\n  sources:\n  - openapi/microsoft-azure-devops-openapi.yml\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://app.vssps.visualstudio.com/oauth2/authorize\n    tokenUrl: https://app.vssps.visualstudio.com/oauth2/token\n    scopes: 4\n  description: Microsoft Entra ID OAuth 2.0\n  sources:\n  - openapi/microsoft-azure-devops-openapi.yml\n  - openapi/microsoft-dynamics-365-openapi.yml\n  - openapi/microsoft-onedrive-openapi.yml\n  - openapi/microsoft-outlook-openapi.yml\n  - openapi/microsoft-power-bi-openapi.yml\n  - openapi/microsoft-power-platform-openapi.yml\n  - openapi/microsoft-sharepoint-openapi.yml\n  -\
  \ openapi/microsoft-teams-openapi.yml\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: api-key\n  description: Azure OpenAI API key\n  sources:\n  - openapi/microsoft-azure-openai-openapi.yml\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://login.microsoftonline.com/{tenantId}/oauth2/v2.0/token\n    scopes: 1\n  description: Microsoft Entra ID OAuth 2.0\n  sources:\n  - openapi/microsoft-azure-openai-openapi.yml\n  - openapi/microsoft-azure-rest-openapi.yml\n  - openapi/microsoft-entra-id-openapi.yml\n  - openapi/microsoft-intune-openapi.yml\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://login.microsoftonline.com/common/oauth2/v2.0/authorize\n    tokenUrl: https://login.microsoftonline.com/common/oauth2/v2.0/token\n    scopes: 20\n  - flow: clientCredentials\n    tokenUrl: https://login.microsoftonline.com/{tenant}/oauth2/v2.0/token\n    scopes: 1\n  description: Microsoft identity\
  \ platform OAuth 2.0 authorization\n  sources:\n  - openapi/microsoft-graph-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/microsoft/refs/heads/main/authentication/microsoft-authentication.yml
summary_line: apiKey/http/oauth2 · 7 schemes
tags:
- Fortune 100
---
