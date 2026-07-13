---
api_key_in:
- header
api_specs:
- filename: azure-document-intelligence-openapi.json
  format: json
  label: Azure AI Document Intelligence REST API
  slug: rest
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/azure-document-intelligence/refs/heads/main/openapi/azure-document-intelligence-openapi.json
auth_types:
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Azure Document Intelligence Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Azure AI Document Intelligence secures its APIs with apiKey and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Azure AI Document Intelligence
provider_slug: azure-document-intelligence
scheme_count: 2
schemes:
- in: header
  name: ApiKeyAuth
  parameter: Ocp-Apim-Subscription-Key
  sources:
  - openapi/azure-document-intelligence-openapi.json
  type: apiKey
- flows:
  - authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize
    flow: authorizationCode
    scopes: 1
    tokenUrl: https://login.microsoftonline.com/common/oauth2/token
  name: OAuth2Auth
  sources:
  - openapi/azure-document-intelligence-openapi.json
  type: oauth2
slug: azure-document-intelligence-authentication
source_filename: azure-document-intelligence-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/azure-document-intelligence-openapi.json\nsummary:\n  types:\n  - apiKey\n  - oauth2\n  api_key_in:\n  - header\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: Ocp-Apim-Subscription-Key\n  sources:\n  - openapi/azure-document-intelligence-openapi.json\n- name: OAuth2Auth\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://login.microsoftonline.com/common/oauth2/authorize\n    tokenUrl: https://login.microsoftonline.com/common/oauth2/token\n    scopes: 1\n  sources:\n  - openapi/azure-document-intelligence-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/azure-document-intelligence/refs/heads/main/authentication/azure-document-intelligence-authentication.yml
summary_line: apiKey/oauth2 · 2 schemes
tags:
- AI
- Document AI
- Azure
- IDP
- OCR
- Microsoft
- REST
---
