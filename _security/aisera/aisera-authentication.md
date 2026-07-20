---
api_key_in:
- header
auth_types:
- oauth2
- http
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Aisera Authentication
name_suffix: Authentication
oauth_flows:
- password
overview: Aisera secures its APIs with oauth2, http, and apiKey across 4 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the password flow(s).
provider_name: Aisera
provider_slug: aisera
scheme_count: 4
schemes:
- description: Tenant/app token that identifies the Aisera app and its System-of-Record data source. Retrieved from Settings > AiseraGPT application details under "Integration Information" (or provided by the Aisera team for User Provisioning). Sent alongside the Authorization header.
  in: header
  name: AppToken
  parameter_name: x-app-token
  type: apiKey
  used_by:
  - Ingestion APIs
  - User Provisioning APIs
- description: 'Bearer access token obtained via OAuth 2.0 Resource Owner Password Credentials grant. POST client_id (app token), username and password (service-account credentials); response returns access_token and expires_in (3600). Presented as "Authorization: Bearer <access_token>".'
  flow: password
  grant_type: password
  name: OAuth2Password
  token_ttl_seconds: 3600
  token_url: https://<tenant>.api.aisera.cloud/tenant-users/oauth2/token
  type: oauth2
  used_by:
  - Ingestion APIs
- description: HTTP Basic authentication using Aisera platform login credentials (base64-encoded). Used by the Data Source Ingestion Monitoring API and accepted by the User Provisioning APIs.
  name: BasicAuth
  scheme: basic
  type: http
  used_by:
  - Data Source Ingestion Monitoring API
  - User Provisioning APIs
- description: Bearer access token (from the OAuth2 password flow) presented in the Authorization header.
  name: BearerAuth
  scheme: bearer
  type: http
  used_by:
  - Ingestion APIs
  - User Provisioning APIs
slug: aisera-authentication
source_filename: aisera-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: searched\nsource: https://docs.aisera.com/apis/apis.md\ndocs: https://docs.aisera.com/apis/apis/ingestion-apis.md\nnote: >-\n  Aisera publishes no OpenAPI specification; this profile is captured from the\n  developer documentation for the Ingestion, Data Source Monitoring, and User\n  Provisioning APIs. API calls are tenant-scoped against\n  https://<tenant>.api.aisera.cloud and https://<company>.login.aisera.cloud.\nsummary:\n  types: [oauth2, http, apiKey]\n  api_key_in: [header]\n  api_key_names: [x-app-token]\n  http_schemes: [basic, bearer]\n  oauth2_flows: [password]\nschemes:\n  - name: AppToken\n    type: apiKey\n    in: header\n    parameter_name: x-app-token\n    description: >-\n      Tenant/app token that identifies the Aisera app and its System-of-Record\n      data source. Retrieved from Settings > AiseraGPT application details under\n      \"Integration Information\" (or provided by the Aisera team for User\n      Provisioning).\
  \ Sent alongside the Authorization header.\n    used_by: [Ingestion APIs, User Provisioning APIs]\n  - name: OAuth2Password\n    type: oauth2\n    flow: password\n    token_url: https://<tenant>.api.aisera.cloud/tenant-users/oauth2/token\n    grant_type: password\n    token_ttl_seconds: 3600\n    description: >-\n      Bearer access token obtained via OAuth 2.0 Resource Owner Password\n      Credentials grant. POST client_id (app token), username and password\n      (service-account credentials); response returns access_token and\n      expires_in (3600). Presented as \"Authorization: Bearer <access_token>\".\n    used_by: [Ingestion APIs]\n  - name: BasicAuth\n    type: http\n    scheme: basic\n    description: >-\n      HTTP Basic authentication using Aisera platform login credentials\n      (base64-encoded). Used by the Data Source Ingestion Monitoring API and\n      accepted by the User Provisioning APIs.\n    used_by: [Data Source Ingestion Monitoring API, User Provisioning APIs]\n\
  \  - name: BearerAuth\n    type: http\n    scheme: bearer\n    description: >-\n      Bearer access token (from the OAuth2 password flow) presented in the\n      Authorization header.\n    used_by: [Ingestion APIs, User Provisioning APIs]\nintegration_auth_note: >-\n  Separately, Aisera supports a broad set of auth types for OUTBOUND connectors\n  to third-party systems (Basic, OAuth 2.0 authorization-code / password /\n  client-credentials, Basic-to-Bearer, Token, JWT, OIDC, OAuth Custom, PAM,\n  No-Auth). Those configure Aisera's data-source integrations, not inbound API\n  authentication, and are documented under\n  https://docs.aisera.com/aisera-platform/adding-data-to-your-tenant/integrations-and-data-sources/supported-auth-types-for-custom-integrations.md\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aisera/refs/heads/main/authentication/aisera-authentication.yml
summary_line: oauth2/http/apiKey · 4 schemes
tags:
- Company
- Agentic AI
- Conversational AI
- IT Service Management
- Customer Service
- Enterprise Search
- AI Copilot
- Knowledge Management
- Workflow Automation
- Large Language Models
---
