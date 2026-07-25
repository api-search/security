---
api_key_in: []
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Akoya Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
overview: Akoya secures its APIs with oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and clientCredentials flow(s).
provider_name: Akoya
provider_slug: akoya
scheme_count: 2
schemes:
- description: Consumer-permissioned data access. The recipient app redirects the consumer to their financial institution's Akoya-hosted authorization server; on consent an authorization code is returned to the app's registered redirect_uri and exchanged at the token endpoint for an id_token + refresh_token. Requires grant_type=authorization_code, the registered redirect_uri, the returned code, and the app's clientId/clientSecret.
  flow: authorizationCode
  grant_type: authorization_code
  name: OAuth2AuthorizationCode
  parameters:
  - grant_type
  - redirect_uri
  - code
  - clientId
  - clientSecret
  source: https://docs.akoya.com/reference/token
  type: oauth2
- description: Service-token (two-legged) authentication for the platform/service APIs — Consent, Apps Management, and Notifications. The recipient presents grant_type=client_credentials with its clientId and clientSecret to obtain a service token used as the bearer on management calls. Scope must include at least one provider (and the relevant product scope, e.g. app_management_v2 for Apps Management, notification_v1 for Notifications).
  flow: clientCredentials
  grant_type: client_credentials
  name: OAuth2ClientCredentials
  parameters:
  - grant_type
  - clientId
  - clientSecret
  - scope
  source: https://docs.akoya.com/reference/token
  type: oauth2
slug: akoya-authentication
source_filename: akoya-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-23'\nmethod: searched\nsource: https://docs.akoya.com/reference/token\ndocs: https://docs.akoya.com/docs/oauth-2\nsummary:\n  types: [oauth2]\n  oauth2_flows: [authorizationCode, clientCredentials]\n  token_types: [id_token, access_token, refresh_token]\n  bearer_token: id_token\n  notes: >-\n    Akoya implements OAuth 2.0 per the FDX standard. Consumers authenticate and grant consent\n    at their own financial institution's authorization server; the id_token returned is used as\n    the bearer token on FDX data-access calls and must be renewed via the refresh_token.\nschemes:\n  - name: OAuth2AuthorizationCode\n    type: oauth2\n    flow: authorizationCode\n    grant_type: authorization_code\n    description: >-\n      Consumer-permissioned data access. The recipient app redirects the consumer to their\n      financial institution's Akoya-hosted authorization server; on consent an authorization\n      code is returned to the app's registered redirect_uri\
  \ and exchanged at the token endpoint\n      for an id_token + refresh_token. Requires grant_type=authorization_code, the registered\n      redirect_uri, the returned code, and the app's clientId/clientSecret.\n    parameters: [grant_type, redirect_uri, code, clientId, clientSecret]\n    source: https://docs.akoya.com/reference/token\n  - name: OAuth2ClientCredentials\n    type: oauth2\n    flow: clientCredentials\n    grant_type: client_credentials\n    description: >-\n      Service-token (two-legged) authentication for the platform/service APIs — Consent, Apps\n      Management, and Notifications. The recipient presents grant_type=client_credentials with\n      its clientId and clientSecret to obtain a service token used as the bearer on management\n      calls. Scope must include at least one provider (and the relevant product scope, e.g.\n      app_management_v2 for Apps Management, notification_v1 for Notifications).\n    parameters: [grant_type, clientId, clientSecret, scope]\n\
  \    source: https://docs.akoya.com/reference/token\nscope_model:\n  note: >-\n    OAuth scope on client-credentials requests must include at least one data-provider scope\n    plus the product/service scope for the API being called (documented examples include\n    app_management_v2 and notification_v1). Data-access scopes are bounded by the consumer's\n    consent grant. Akoya does not publish a full downloadable scope reference; scopes are\n    provisioned per app in the Data Recipient Hub.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/akoya/refs/heads/main/authentication/akoya-authentication.yml
summary_line: oauth2 · 2 schemes
tags:
- Fintech
- Open Banking
- Open Finance
- Aggregator
- Data Access Network
- Tokenized
- Consumer-Permissioned
- FDX
- Account Aggregation
- United States
---
