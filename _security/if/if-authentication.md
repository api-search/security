---
api_key_in: []
auth_types:
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
method: searched
name: If Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: IF secures its APIs with oauth2 and openIdConnect across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: IF
provider_slug: if
scheme_count: 2
schemes:
- description: OAuth 2.0 client-credentials flow with a JWT client assertion. The client generates an RSA key pair (4096-bit) and a self-signed certificate; the public key certificate is registered with the IF team, which issues a client ID. The client requests a short-lived access token from the Keycloak token endpoint and presents it as a Bearer token on every API call.
  flows:
  - flow: clientCredentials
    tokenUrl: https://account.integrated.finance/auth/realms/ifp/protocol/openid-connect/token
  header: 'Authorization: Bearer <access_token>'
  name: OAuth2
  sources:
  - https://developer.integrated.finance/docs/authentication
  type: oauth2
- issuer: https://account.integrated.finance/auth/realms/ifp
  name: OpenIDConnect
  openIdConnectUrl: https://account.integrated.finance/auth/realms/ifp/.well-known/openid-configuration
  sandbox_openIdConnectUrl: https://sandbox-account.integrated.finance/auth/realms/ifp/.well-known/openid-configuration
  sources:
  - well-known/if-openid-configuration.json
  type: openIdConnect
slug: if-authentication
source_filename: if-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://developer.integrated.finance/docs/authentication\ndocs: https://developer.integrated.finance/docs/authentication\nsummary:\n  types: [oauth2, openIdConnect]\n  oauth2_flows: [clientCredentials]\n  client_authentication: private_key_jwt\n  token_type: Bearer\n  identity_provider: Keycloak (realm \"ifp\")\nschemes:\n- name: OAuth2\n  type: oauth2\n  description: >-\n    OAuth 2.0 client-credentials flow with a JWT client assertion. The client\n    generates an RSA key pair (4096-bit) and a self-signed certificate; the public\n    key certificate is registered with the IF team, which issues a client ID. The\n    client requests a short-lived access token from the Keycloak token endpoint and\n    presents it as a Bearer token on every API call.\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://account.integrated.finance/auth/realms/ifp/protocol/openid-connect/token\n  header: 'Authorization: Bearer <access_token>'\n\
  \  sources: [https://developer.integrated.finance/docs/authentication]\n- name: OpenIDConnect\n  type: openIdConnect\n  openIdConnectUrl: https://account.integrated.finance/auth/realms/ifp/.well-known/openid-configuration\n  sandbox_openIdConnectUrl: https://sandbox-account.integrated.finance/auth/realms/ifp/.well-known/openid-configuration\n  issuer: https://account.integrated.finance/auth/realms/ifp\n  sources: [well-known/if-openid-configuration.json]\nenvironments:\n  production:\n    issuer: https://account.integrated.finance/auth/realms/ifp\n    token_endpoint: https://account.integrated.finance/auth/realms/ifp/protocol/openid-connect/token\n    api_base: https://api.integrated.finance\n  sandbox:\n    issuer: https://sandbox-account.integrated.finance/auth/realms/ifp\n    token_endpoint: https://sandbox-account.integrated.finance/auth/realms/ifp/protocol/openid-connect/token\n    api_base: https://sandbox-api.integrated.finance\ntransport_security: HTTPS with TLS v1.2 or above required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/if/refs/heads/main/authentication/if-authentication.yml
summary_line: oauth2/openIdConnect · 2 schemes
tags:
- Company
- Financial Services
- Embedded Finance
- Banking as a Service
- Payments
- Cards
- Foreign Exchange
- Compliance
- Open Banking
- API
---
