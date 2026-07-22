---
api_key_in:
- header
auth_types:
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Tecton Databricks Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Tecton (Databricks) secures its APIs with apiKey and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Tecton (Databricks)
provider_slug: tecton-databricks
scheme_count: 2
schemes:
- description: API-key authentication for the Feature Service HTTP API. The key is passed as an Authorization header with the "Tecton-key" prefix. Keys are issued to Service Accounts; newly created credentials can take up to 60 seconds to activate.
  docs: https://docs.tecton.ai/http-api
  format: 'Authorization: Tecton-key <YOUR-API-KEY>'
  header: Authorization
  in: header
  name: TectonKey
  type: apiKey
- description: Service Accounts authenticate with OAuth 2.0 Client Credentials. The Service Account ID and an active client secret are exchanged at the tokens endpoint (scope "everything") for an access token, which is then used to call Tecton APIs. Client Credentials cannot call Tecton APIs directly; they must first be exchanged for an access token.
  docs: https://docs.tecton.ai/docs/beta/setting-up-tecton/administration-setup/programmatic-access-using-service-accounts
  flow: clientCredentials
  name: ServiceAccountOAuth
  scopes:
  - everything
  type: oauth2
slug: tecton-databricks-authentication
source_filename: tecton-databricks-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://docs.tecton.ai/docs/beta/setting-up-tecton/administration-setup/programmatic-access-using-service-accounts\ndocs: https://docs.tecton.ai/http-api\nsummary:\n  types: [apiKey, oauth2]\n  api_key_in: [header]\n  oauth2_flows: [clientCredentials]\nschemes:\n  - name: TectonKey\n    type: apiKey\n    in: header\n    header: Authorization\n    format: 'Authorization: Tecton-key <YOUR-API-KEY>'\n    description: >-\n      API-key authentication for the Feature Service HTTP API. The key is passed as an\n      Authorization header with the \"Tecton-key\" prefix. Keys are issued to Service\n      Accounts; newly created credentials can take up to 60 seconds to activate.\n    docs: https://docs.tecton.ai/http-api\n  - name: ServiceAccountOAuth\n    type: oauth2\n    flow: clientCredentials\n    description: >-\n      Service Accounts authenticate with OAuth 2.0 Client Credentials. The Service Account ID\n      and an active client\
  \ secret are exchanged at the tokens endpoint (scope \"everything\")\n      for an access token, which is then used to call Tecton APIs. Client Credentials cannot\n      call Tecton APIs directly; they must first be exchanged for an access token.\n    scopes:\n      - everything\n    docs: https://docs.tecton.ai/docs/beta/setting-up-tecton/administration-setup/programmatic-access-using-service-accounts\nnotes: >-\n  Authorization is role-based - Service Accounts require Consumer/Editor privileges on a\n  Feature Service (a 403 \"Not Authorized\" is returned otherwise). SCIM 2.0 is supported for\n  user/group provisioning.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tecton-databricks/refs/heads/main/authentication/tecton-databricks-authentication.yml
summary_line: apiKey/oauth2 · 2 schemes
tags:
- Company
- Ai Infrastructure
- Feature Store
- Feature Platform
- Machine Learning
- MLOps
- Real Time
- Databricks
---
