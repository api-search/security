---
api_key_in: []
auth_types: []
description: Authentication profile for the Teads developer APIs. Both public REST surfaces use static, long-lived API-key style credentials issued out of band — via Teads Ad Manager or a Teads account representative. No OAuth 2.0, OpenID Connect, mTLS, JWT, signing scheme, scope model, expiry or documented rotation path exists on any surface, and there is no self-serve credential issuance.
kind: authentication
layout: security
method: searched
name: Teads Authentication
name_suffix: Authentication
oauth_flows: []
overview: Teads declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: Teads
provider_slug: teads
scheme_count: 0
schemes: []
slug: teads-authentication
source_filename: teads-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: https://developers.teads.com/docs/Chatbot-AI-SDK/Getting-Started/integration-guide/\ndescription: >-\n  Authentication profile for the Teads developer APIs. Both public REST surfaces\n  use static, long-lived API-key style credentials issued out of band — via Teads\n  Ad Manager or a Teads account representative. No OAuth 2.0, OpenID Connect,\n  mTLS, JWT, signing scheme, scope model, expiry or documented rotation path\n  exists on any surface, and there is no self-serve credential issuance.\napis:\n- name: Teads Conversions API\n  base: https://ca.teads.tv\n  schemes:\n  - type: apiKey\n    name: Conversion API Token\n    in: token\n    location: request payload / connector configuration\n    provisioning: >-\n      Generated in Teads Ad Manager under Settings > Conversion API Tokens >\n      Generate Conversion API Token. Shown once; must be stored securely.\n    rotation: not documented\n    expiry: not documented\n    scopes:\
  \ none\n    docs: https://docs.tealium.com/server-side-connectors/teads-conversions-connector/\n  companion_identifiers:\n    note: >-\n      Server-side events are correlated with browser activity through Teads\n      first-party cookies rather than an auth mechanism.\n    cookies:\n    - tfpai (carries auctid, the event/click id)\n    - tfpvi (user identifier)\n    - tfpsi (user session id)\n- name: Teads In-Chat Recommendations API\n  base: https://mv.outbrain.com/Multivac/api/in-chat-recs\n  schemes:\n  - type: apiKey\n    name: key\n    in: query\n    provisioning: >-\n      Unique Partner API Key obtained from a Teads account representative,\n      alongside an approved Widget ID (e.g. APP_12). Passed as the `key` query\n      parameter.\n    rotation: not documented\n    expiry: not documented\n    scopes: none\n    env_var: TEADS_API_KEY\n    docs: https://developers.teads.com/docs/Chatbot-AI-SDK/Getting-Started/integration-guide/\n    risk: >-\n      A credential in the query\
  \ string is written to proxy, CDN and server access\n      logs and to browser referrer chains. Teads' own settings page tells\n      integrators to keep the key in environment variables or secrets management\n      and never to hardcode it client-side, but the transport itself puts it in\n      the URL. A header-based credential would be the single largest security\n      improvement available on this surface.\n  required_request_context:\n    note: >-\n      Not authentication, but mandatory alongside it — the caller must forward\n      the END USER's context rather than the server's, and the API is documented\n      to depend on it for geo-compliance and fraud prevention.\n    headers:\n    - name: User-Agent\n      value: the end user's agent string\n    - name: X-Forwarded-For\n      value: the end user's masked or full IP address\n  consent_parameters:\n    note: >-\n      Requests carry regulatory consent signals in addition to the credential;\n      absent or malformed values affect\
  \ eligibility, not authentication.\n    parameters:\n    - name: api_consent\n      requirement: recommended\n      detail: Set to 1 when the host app has obtained user consent.\n    - name: cnsntv2\n      requirement: required in the EU\n      detail: IAB TCF v2.0 consent string.\n    docs: https://developers.teads.com/docs/Chatbot-AI-SDK/Getting-Started/privacy-guide/\n- name: Teads Ad Manager (console)\n  base: https://login.teads.tv/login\n  schemes:\n  - type: interactive\n    name: Teads Ad Manager login\n    note: >-\n      Human console login where Conversion API Tokens are generated. No public\n      API for credential management is documented.\nmobile_sdk_credentials:\n  note: >-\n    The mobile SDKs are not authenticated with a secret. Placement identity is\n    the credential surface.\n  identifiers:\n  - pid (Teads placement id, numeric)\n  - widgetId + installationKey (Feed / Recommendations placements)\n  test_values: see sandbox/teads-sandbox.yml\nabsent:\n  oauth2: true\n\
  \  oidc: true\n  mutual_tls: true\n  jwt: true\n  request_signing: true\n  scopes: true\n  token_expiry: true\n  documented_rotation: true\n  self_serve_issuance: true\n  well_known_discovery: >-\n    /.well-known/openid-configuration and /.well-known/oauth-authorization-server\n    return 404 on developers.teads.com, ca.teads.tv and mv.outbrain.com.\nnotes: >-\n  No OpenAPI document is published by Teads, so this profile is transcribed from\n  the developer portal, the In-Chat API settings/privacy pages and partner\n  integration documentation rather than from securitySchemes in a machine spec.\n  scopes/ is intentionally not emitted for this provider — there is no OAuth\n  surface for scopes to describe.\ncross_links:\n  conventions: conventions/teads-conventions.yml\n  scopes: null\n  security: security/teads-trust-center.yml\nchecked: '2026-08-13'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/teads/refs/heads/main/authentication/teads-authentication.yml
summary_line: 0 schemes
tags:
- Company
- Advertising
- AdTech
- Advertising Technology
- Video Advertising
- Conversions API
- Contextual Advertising
- Mobile SDK
- Conversational AI
---
