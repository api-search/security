---
api_key_in:
- header
auth_types:
- openIdConnect
- oauth2
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Blackpoint Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
- deviceCode
- refreshToken
overview: Blackpoint secures its APIs with openIdConnect, oauth2, and apiKey across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode, clientCredentials, deviceCode, and refreshToken flow(s).
provider_name: Blackpoint
provider_slug: blackpoint
scheme_count: 2
schemes:
- audience: https://bpsnap.auth0.com/api/v2/
  authorizationUrl: https://login.bpsnap.com/authorize
  deviceAuthorizationUrl: https://login.bpsnap.com/oauth/device/code
  grant_types:
  - authorization_code
  - client_credentials
  - refresh_token
  - urn:ietf:params:oauth:grant-type:device_code
  - urn:ietf:params:oauth:grant-type:token-exchange
  issuer: https://login.bpsnap.com/
  jwksUri: https://login.bpsnap.com/.well-known/jwks.json
  name: CompassOneOIDC
  openIdConnectUrl: https://login.bpsnap.com/.well-known/openid-configuration
  provider: Auth0
  tokenUrl: https://login.bpsnap.com/oauth/token
  type: openIdConnect
  userinfoUrl: https://login.bpsnap.com/userinfo
- description: Secret API key generated in the CompassOne portal, sent in an Authorization header for programmatic access (e.g. the PSCompassOne PowerShell module's Connect-CompassOne -ApiKey).
  in: header
  name: CompassOneApiKey
  parameter_name: Authorization
  type: apiKey
slug: blackpoint-authentication
source_filename: blackpoint-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: >-\n  https://login.bpsnap.com/.well-known/openid-configuration (Auth0 OIDC\n  discovery for Blackpoint's identity tenant, referenced by the CompassOne app\n  as WEB_PUBLIC_AUTH0_DOMAIN); CompassOne API key model documented via the\n  BlackpointCyber/PSCompassOne module (Connect-CompassOne -ApiKey).\ndocs: https://login.bpsnap.com/.well-known/openid-configuration\nsummary:\n  types: [openIdConnect, oauth2, apiKey]\n  api_key_in: [header]\n  oauth2_flows: [authorizationCode, clientCredentials, deviceCode, refreshToken]\nschemes:\n- name: CompassOneOIDC\n  type: openIdConnect\n  openIdConnectUrl: https://login.bpsnap.com/.well-known/openid-configuration\n  issuer: https://login.bpsnap.com/\n  provider: Auth0\n  authorizationUrl: https://login.bpsnap.com/authorize\n  tokenUrl: https://login.bpsnap.com/oauth/token\n  deviceAuthorizationUrl: https://login.bpsnap.com/oauth/device/code\n  userinfoUrl: https://login.bpsnap.com/userinfo\n\
  \  jwksUri: https://login.bpsnap.com/.well-known/jwks.json\n  audience: https://bpsnap.auth0.com/api/v2/\n  grant_types:\n  - authorization_code\n  - client_credentials\n  - refresh_token\n  - urn:ietf:params:oauth:grant-type:device_code\n  - urn:ietf:params:oauth:grant-type:token-exchange\n- name: CompassOneApiKey\n  type: apiKey\n  in: header\n  parameter_name: Authorization\n  description: >-\n    Secret API key generated in the CompassOne portal, sent in an Authorization\n    header for programmatic access (e.g. the PSCompassOne PowerShell module's\n    Connect-CompassOne -ApiKey).\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/blackpoint/refs/heads/main/authentication/blackpoint-authentication.yml
summary_line: openIdConnect/oauth2/apiKey · 2 schemes
tags:
- Company
- Cybersecurity
- Managed Detection and Response
- MDR
- Security Operations
- Identity Threat Detection
- Security Posture Management
- MSP
- SIEM
---
