---
api_key_in: []
auth_types:
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
method: probed
name: Amerisourcebergen Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: AmerisourceBergen secures its APIs with oauth2 and openIdConnect across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: AmerisourceBergen
provider_slug: amerisourcebergen
scheme_count: 2
schemes:
- client_id_observed: sb-dev-portal-xsuaa!b33
  flows:
  - authorizationUrl: https://ab-cloud-foundry-prd.authentication.us21.hana.ondemand.com/oauth/authorize
    flow: authorizationCode
    pkce_challenge_methods:
    - S256
    tokenUrl: https://ab-cloud-foundry-prd.authentication.us21.hana.ondemand.com/oauth/token
  name: SAP XSUAA (Cencora developer portal)
  redirect_uri_observed: https://api.cencora.com/login/callback
  sources:
  - https://api.cencora.com/
  type: oauth2
- end_session_endpoint: https://ab-cloud-foundry-prd.authentication.us21.hana.ondemand.com/logout.do
  id_token_signing_alg_values_supported:
  - RS256
  - HS256
  issuer: https://ab-cloud-foundry-prd.authentication.us21.hana.ondemand.com/oauth/token
  jwks_uri: https://ab-cloud-foundry-prd.authentication.us21.hana.ondemand.com/token_keys
  name: SAP XSUAA OIDC
  openIdConnectUrl: https://ab-cloud-foundry-prd.authentication.us21.hana.ondemand.com/.well-known/openid-configuration
  sources:
  - well-known/amerisourcebergen-openid-configuration.json
  token_endpoint_auth_methods_supported:
  - client_secret_basic
  - client_secret_post
  - tls_client_auth
  type: openIdConnect
  userinfo_endpoint: https://ab-cloud-foundry-prd.authentication.us21.hana.ondemand.com/userinfo
slug: amerisourcebergen-authentication
source_filename: amerisourcebergen-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-02'\nmethod: probed\nsource: >-\n  https://api.cencora.com/ (observed OAuth redirect) and\n  https://ab-cloud-foundry-prd.authentication.us21.hana.ondemand.com/.well-known/openid-configuration\ndocs: null\nnote: >-\n  Derived from live probes, not from an OpenAPI — Cencora publishes no machine-readable\n  contract. api.cencora.com is a Cencora-operated SAP API Business Hub Enterprise developer\n  portal (DNS CNAME ab-cloud-foundry-prd.apibhubenterprise.cfapps.us21.hana.ondemand.com).\n  Every request to it, on every path, returns an HTML shim that redirects the browser to the\n  SAP XSUAA authorization server with response_type=code, client_id=sb-dev-portal-xsuaa!b33\n  and code_challenge_method=S256. That is the whole of the observable auth surface: there is\n  no anonymous API, no API-key issuance page, and no published token-acquisition guide.\nsummary:\n  types:\n    - oauth2\n    - openIdConnect\n  api_key_in: []\n  oauth2_flows:\n    - authorizationCode\n\
  \  pkce: S256\n  anonymous_access: false\nschemes:\n  - name: SAP XSUAA (Cencora developer portal)\n    type: oauth2\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://ab-cloud-foundry-prd.authentication.us21.hana.ondemand.com/oauth/authorize\n        tokenUrl: https://ab-cloud-foundry-prd.authentication.us21.hana.ondemand.com/oauth/token\n        pkce_challenge_methods: [S256]\n    client_id_observed: sb-dev-portal-xsuaa!b33\n    redirect_uri_observed: https://api.cencora.com/login/callback\n    sources:\n      - https://api.cencora.com/\n  - name: SAP XSUAA OIDC\n    type: openIdConnect\n    openIdConnectUrl: https://ab-cloud-foundry-prd.authentication.us21.hana.ondemand.com/.well-known/openid-configuration\n    issuer: https://ab-cloud-foundry-prd.authentication.us21.hana.ondemand.com/oauth/token\n    jwks_uri: https://ab-cloud-foundry-prd.authentication.us21.hana.ondemand.com/token_keys\n    userinfo_endpoint: https://ab-cloud-foundry-prd.authentication.us21.hana.ondemand.com/userinfo\n\
  \    end_session_endpoint: https://ab-cloud-foundry-prd.authentication.us21.hana.ondemand.com/logout.do\n    token_endpoint_auth_methods_supported:\n      - client_secret_basic\n      - client_secret_post\n      - tls_client_auth\n    id_token_signing_alg_values_supported: [RS256, HS256]\n    sources:\n      - well-known/amerisourcebergen-openid-configuration.json\ngaps:\n  - >-\n    No public documentation of how a developer obtains credentials for the portal —\n    account provisioning appears to be a customer/partner motion, not self-service.\n  - >-\n    No protected-resource metadata (RFC 9728) is served at api.cencora.com, so an agent\n    cannot discover the authorization server from the resource.\nx-evidence:\n  checked: '2026-09-02'\n  probes:\n    - url: https://api.cencora.com/\n      http_status: 200\n      note: 858-byte HTML OAuth redirect shim; identical body on every path probed\n    - url: https://ab-cloud-foundry-prd.authentication.us21.hana.ondemand.com/.well-known/openid-configuration\n\
  \      http_status: 200\n      content_type: application/json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amerisourcebergen/refs/heads/main/authentication/amerisourcebergen-authentication.yml
summary_line: oauth2/openIdConnect · 2 schemes
tags:
- Pharmaceutical Distribution
- Healthcare
- Drug Distribution
- Manufacturer Solutions
- Provider Solutions
- Animal Health
- Life Sciences
- Fortune 100
---
