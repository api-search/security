---
api_key_in: []
auth_types:
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
method: searched
name: Proemion Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Proemion secures its APIs with oauth2 and openIdConnect across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Proemion
provider_slug: proemion
scheme_count: 2
schemes:
- issuer: https://dataportal.proemion.com/auth/realms/af0b450b-63cb-4f6e-a994-bdab447c64ba
  name: OpenIDConnect
  openIdConnectUrl: https://api.proemion.com/.well-known/openid-configuration
  sources:
  - well-known/proemion-openid-configuration.json
  type: openIdConnect
- flows:
  - authorizationUrl: https://dataportal.proemion.com/auth/realms/af0b450b-63cb-4f6e-a994-bdab447c64ba/protocol/openid-connect/auth
    flow: clientCredentials
    tokenUrl: https://dataportal.proemion.com/auth/realms/af0b450b-63cb-4f6e-a994-bdab447c64ba/protocol/openid-connect/token
  name: OAuth2
  sources:
  - well-known/proemion-openid-configuration.json
  token_endpoint_auth_methods:
  - private_key_jwt
  - client_secret_basic
  - client_secret_post
  - tls_client_auth
  - client_secret_jwt
  type: oauth2
slug: proemion-authentication
source_filename: proemion-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://api.proemion.com/.well-known/openid-configuration\ndocs: https://docs.proemion.com/docs/dataportal/organization_structure/#api-client-management\nsummary:\n  types: [oauth2, openIdConnect]\n  oauth2_flows: [clientCredentials]\n  note: >-\n    The DataPlatform REST API authenticates with OAuth2 API client credentials\n    (client_id + client_secret) issued from the DataPortal under\n    Organization > API Client management. Tokens are issued by a Keycloak\n    OpenID Connect provider. User credentials are not accepted for the API.\nschemes:\n- name: OpenIDConnect\n  type: openIdConnect\n  openIdConnectUrl: https://api.proemion.com/.well-known/openid-configuration\n  issuer: https://dataportal.proemion.com/auth/realms/af0b450b-63cb-4f6e-a994-bdab447c64ba\n  sources: [well-known/proemion-openid-configuration.json]\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://dataportal.proemion.com/auth/realms/af0b450b-63cb-4f6e-a994-bdab447c64ba/protocol/openid-connect/token\n\
  \    authorizationUrl: https://dataportal.proemion.com/auth/realms/af0b450b-63cb-4f6e-a994-bdab447c64ba/protocol/openid-connect/auth\n  token_endpoint_auth_methods:\n  - private_key_jwt\n  - client_secret_basic\n  - client_secret_post\n  - tls_client_auth\n  - client_secret_jwt\n  sources: [well-known/proemion-openid-configuration.json]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/proemion/refs/heads/main/authentication/proemion-authentication.yml
summary_line: oauth2/openIdConnect · 2 schemes
tags:
- Company
- Telematics
- IoT
- Off-Highway Equipment
- CAN Bus
- Fleet Management
- Machine Data
- OEM
- AEMP
- Construction
- Agriculture
---
