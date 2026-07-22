---
api_key_in: []
auth_types:
- http
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
method: searched
name: Ubio Automation Cloud Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: UBIO Automation Cloud secures its APIs with http, oauth2, and openIdConnect across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: UBIO Automation Cloud
provider_slug: ubio-automation-cloud
scheme_count: 3
schemes:
- description: App Secret Key obtained from the Automation Cloud dashboard, sent as the username of an HTTP Basic credential (no password). A short-lived Job Access Token retrieved via getAccessToken() can be used the same way for browser-side access to a single job.
  name: appSecretKey
  scheme: basic
  sources:
  - https://github.com/automationcloud/client-javascript/blob/master/src/main/ac-request.ts
  type: http
- description: OAuth2 client credentials (clientId + clientSecret) issued for the automationcloud Keycloak realm; the client library exchanges them for bearer tokens against the realm token endpoint.
  flows:
  - flow: clientCredentials
    scopes: {}
    tokenUrl: https://auth.automationcloud.net/auth/realms/automationcloud/protocol/openid-connect/token
  name: oauth2ClientCredentials
  sources:
  - https://github.com/automationcloud/client-javascript/blob/master/src/main/ac-request.ts
  type: oauth2
- description: Keycloak OIDC discovery for the automationcloud realm. Grant types advertised include authorization_code, implicit, refresh_token, password, and client_credentials; token endpoint auth methods include private_key_jwt, client_secret_basic, client_secret_post, tls_client_auth, and client_secret_jwt.
  name: openIdConnect
  openIdConnectUrl: https://auth.automationcloud.net/auth/realms/automationcloud/.well-known/openid-configuration
  sources:
  - well-known/ubio-automation-cloud-openid-configuration.json
  type: openIdConnect
slug: ubio-automation-cloud-authentication
source_filename: ubio-automation-cloud-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://github.com/automationcloud/client-javascript/blob/master/src/main/ac-request.ts\ndocs: https://auth.automationcloud.net/auth/realms/automationcloud/.well-known/openid-configuration\nsummary:\n  types:\n  - http\n  - oauth2\n  - openIdConnect\n  http_schemes:\n  - basic\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: appSecretKey\n  type: http\n  scheme: basic\n  description: App Secret Key obtained from the Automation Cloud dashboard, sent\n    as the username of an HTTP Basic credential (no password). A short-lived Job\n    Access Token retrieved via getAccessToken() can be used the same way for browser-side\n    access to a single job.\n  sources:\n  - https://github.com/automationcloud/client-javascript/blob/master/src/main/ac-request.ts\n- name: oauth2ClientCredentials\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://auth.automationcloud.net/auth/realms/automationcloud/protocol/openid-connect/token\n\
  \    scopes: {}\n  description: OAuth2 client credentials (clientId + clientSecret) issued for the\n    automationcloud Keycloak realm; the client library exchanges them for bearer\n    tokens against the realm token endpoint.\n  sources:\n  - https://github.com/automationcloud/client-javascript/blob/master/src/main/ac-request.ts\n- name: openIdConnect\n  type: openIdConnect\n  openIdConnectUrl: https://auth.automationcloud.net/auth/realms/automationcloud/.well-known/openid-configuration\n  description: Keycloak OIDC discovery for the automationcloud realm. Grant types\n    advertised include authorization_code, implicit, refresh_token, password, and\n    client_credentials; token endpoint auth methods include private_key_jwt, client_secret_basic,\n    client_secret_post, tls_client_auth, and client_secret_jwt.\n  sources:\n  - well-known/ubio-automation-cloud-openid-configuration.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ubio-automation-cloud/refs/heads/main/authentication/ubio-automation-cloud-authentication.yml
summary_line: http/oauth2/openIdConnect · 3 schemes
tags:
- Automation
- Web Automation
- RPA
- Travel
- Booking
- Jobs
- Company
---
