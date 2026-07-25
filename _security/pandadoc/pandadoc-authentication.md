---
api_key_in:
- header
api_specs:
- filename: pandadoc-api-logs-api-openapi.yml
  format: yaml
  label: PandaDoc API Logs API
  slug: pandadoc-api-logs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pandadoc/refs/heads/main/openapi/pandadoc-api-logs-api-openapi.yml
- filename: pandadoc-contacts-api-openapi.yml
  format: yaml
  label: PandaDoc Contacts API
  slug: pandadoc-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pandadoc/refs/heads/main/openapi/pandadoc-contacts-api-openapi.yml
- filename: pandadoc-document-attachments-api-openapi.yml
  format: yaml
  label: PandaDoc Document Attachments API
  slug: pandadoc-document-attachments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pandadoc/refs/heads/main/openapi/pandadoc-document-attachments-api-openapi.yml
- filename: pandadoc-document-fields-api-openapi.yml
  format: yaml
  label: PandaDoc Document Fields API
  slug: pandadoc-document-fields-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pandadoc/refs/heads/main/openapi/pandadoc-document-fields-api-openapi.yml
- filename: pandadoc-document-link-to-crm-api-openapi.yml
  format: yaml
  label: PandaDoc Document Link to CRM API
  slug: pandadoc-document-link-to-crm-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pandadoc/refs/heads/main/openapi/pandadoc-document-link-to-crm-api-openapi.yml
- filename: pandadoc-document-recipients-api-openapi.yml
  format: yaml
  label: PandaDoc Document Recipients API
  slug: pandadoc-document-recipients-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pandadoc/refs/heads/main/openapi/pandadoc-document-recipients-api-openapi.yml
- filename: pandadoc-document-reminders-api-openapi.yml
  format: yaml
  label: PandaDoc Document Reminders API
  slug: pandadoc-document-reminders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pandadoc/refs/heads/main/openapi/pandadoc-document-reminders-api-openapi.yml
- filename: pandadoc-documents-api-openapi.yml
  format: yaml
  label: PandaDoc Documents API
  slug: pandadoc-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pandadoc/refs/heads/main/openapi/pandadoc-documents-api-openapi.yml
- filename: pandadoc-folders-api-openapi.yml
  format: yaml
  label: PandaDoc Folders API
  slug: pandadoc-folders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pandadoc/refs/heads/main/openapi/pandadoc-folders-api-openapi.yml
- filename: pandadoc-forms-api-openapi.yml
  format: yaml
  label: PandaDoc Forms API
  slug: pandadoc-forms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pandadoc/refs/heads/main/openapi/pandadoc-forms-api-openapi.yml
- filename: pandadoc-members-api-openapi.yml
  format: yaml
  label: PandaDoc Members API
  slug: pandadoc-members-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pandadoc/refs/heads/main/openapi/pandadoc-members-api-openapi.yml
- filename: pandadoc-templates-api-openapi.yml
  format: yaml
  label: PandaDoc Templates API
  slug: pandadoc-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pandadoc/refs/heads/main/openapi/pandadoc-templates-api-openapi.yml
- filename: pandadoc-webhook-events-api-openapi.yml
  format: yaml
  label: PandaDoc Webhook Events API
  slug: pandadoc-webhook-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pandadoc/refs/heads/main/openapi/pandadoc-webhook-events-api-openapi.yml
- filename: pandadoc-webhook-subscriptions-api-openapi.yml
  format: yaml
  label: PandaDoc Webhook Subscriptions API
  slug: pandadoc-webhook-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pandadoc/refs/heads/main/openapi/pandadoc-webhook-subscriptions-api-openapi.yml
- filename: pandadoc-workspaces-api-openapi.yml
  format: yaml
  label: PandaDoc Workspaces API
  slug: pandadoc-workspaces-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pandadoc/refs/heads/main/openapi/pandadoc-workspaces-api-openapi.yml
auth_types:
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Pandadoc Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: PandaDoc secures its APIs with apiKey and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: PandaDoc
provider_slug: pandadoc
scheme_count: 2
schemes:
- description: API Key authentication. Include the key in the Authorization header as "API-Key YOUR_API_KEY". Generate keys from the PandaDoc Developer Dashboard.
  in: header
  name: apiKey
  parameter: Authorization
  sources:
  - openapi/pandadoc-rest-api-openapi.yml
  type: apiKey
- description: OAuth 2.0 authentication. Use the authorization code flow to obtain user-scoped access tokens. Tokens expire after approximately one year.
  flows:
  - authorizationUrl: https://app.pandadoc.com/oauth2/authorize
    flow: authorizationCode
    scopes: 2
    tokenUrl: https://api.pandadoc.com/oauth2/access_token
  name: oauth2
  sources:
  - openapi/pandadoc-rest-api-openapi.yml
  type: oauth2
slug: pandadoc-authentication
source_filename: pandadoc-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/pandadoc-rest-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - oauth2\n  api_key_in:\n  - header\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: API Key authentication. Include the key in the Authorization header as \"API-Key\n    YOUR_API_KEY\". Generate keys from the PandaDoc Developer Dashboard.\n  sources:\n  - openapi/pandadoc-rest-api-openapi.yml\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://app.pandadoc.com/oauth2/authorize\n    tokenUrl: https://api.pandadoc.com/oauth2/access_token\n    scopes: 2\n  description: OAuth 2.0 authentication. Use the authorization code flow to obtain user-scoped\n    access tokens. Tokens expire after approximately one year.\n  sources:\n  - openapi/pandadoc-rest-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pandadoc/refs/heads/main/authentication/pandadoc-authentication.yml
summary_line: apiKey/oauth2 · 2 schemes
tags:
- Document Automation
- E-Signature
- Document Management
- Document Generation
- Webhooks
---
