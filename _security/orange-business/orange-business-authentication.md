---
api_key_in:
- header
api_specs:
- filename: orange-business-live-objects-openapi.json
  format: json
  label: Orange Business Live Objects API
  slug: orange-business-live-objects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orange-business/refs/heads/main/openapi/orange-business-live-objects-openapi.json
- filename: orange-business-check-device-swap-api-openapi.yml
  format: yaml
  label: Orange Business Check Device Swap API
  slug: orange-business-check-device-swap-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orange-business/refs/heads/main/openapi/orange-business-check-device-swap-api-openapi.yml
- filename: orange-business-check-sim-swap-api-openapi.yml
  format: yaml
  label: Orange Business Check SIM swap API
  slug: orange-business-check-sim-swap-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orange-business/refs/heads/main/openapi/orange-business-check-sim-swap-api-openapi.yml
- filename: orange-business-device-reachability-status-api-openapi.yml
  format: yaml
  label: Orange Business Device reachability status API
  slug: orange-business-device-reachability-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orange-business/refs/heads/main/openapi/orange-business-device-reachability-status-api-openapi.yml
- filename: orange-business-geofencing-subscriptions-api-openapi.yml
  format: yaml
  label: Orange Business Geofencing subscriptions API
  slug: orange-business-geofencing-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orange-business/refs/heads/main/openapi/orange-business-geofencing-subscriptions-api-openapi.yml
- filename: orange-business-location-retrieval-api-openapi.yml
  format: yaml
  label: Orange Business Location retrieval API
  slug: orange-business-location-retrieval-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orange-business/refs/heads/main/openapi/orange-business-location-retrieval-api-openapi.yml
- filename: orange-business-location-verification-api-openapi.yml
  format: yaml
  label: Orange Business Location verification API
  slug: orange-business-location-verification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orange-business/refs/heads/main/openapi/orange-business-location-verification-api-openapi.yml
- filename: orange-business-match-api-openapi.yml
  format: yaml
  label: Orange Business Match API
  slug: orange-business-match-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orange-business/refs/heads/main/openapi/orange-business-match-api-openapi.yml
- filename: orange-business-phone-number-share-api-openapi.yml
  format: yaml
  label: Orange Business Phone number share API
  slug: orange-business-phone-number-share-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orange-business/refs/heads/main/openapi/orange-business-phone-number-share-api-openapi.yml
- filename: orange-business-phone-number-verify-api-openapi.yml
  format: yaml
  label: Orange Business Phone number verify API
  slug: orange-business-phone-number-verify-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orange-business/refs/heads/main/openapi/orange-business-phone-number-verify-api-openapi.yml
- filename: orange-business-population-density-data-api-openapi.yml
  format: yaml
  label: Orange Business Population Density Data API
  slug: orange-business-population-density-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orange-business/refs/heads/main/openapi/orange-business-population-density-data-api-openapi.yml
- filename: orange-business-qos-sessions-api-openapi.yml
  format: yaml
  label: Orange Business QoS Sessions API
  slug: orange-business-qos-sessions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orange-business/refs/heads/main/openapi/orange-business-qos-sessions-api-openapi.yml
- filename: orange-business-retrieve-device-swap-date-api-openapi.yml
  format: yaml
  label: Orange Business Retrieve Device Swap Date API
  slug: orange-business-retrieve-device-swap-date-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orange-business/refs/heads/main/openapi/orange-business-retrieve-device-swap-date-api-openapi.yml
- filename: orange-business-retrieve-sim-swap-date-api-openapi.yml
  format: yaml
  label: Orange Business Retrieve SIM swap date API
  slug: orange-business-retrieve-sim-swap-date-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orange-business/refs/heads/main/openapi/orange-business-retrieve-sim-swap-date-api-openapi.yml
- filename: orange-business-roaming-status-retrieval-api-openapi.yml
  format: yaml
  label: Orange Business Roaming status retrieval API
  slug: orange-business-roaming-status-retrieval-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orange-business/refs/heads/main/openapi/orange-business-roaming-status-retrieval-api-openapi.yml
auth_types:
- apiKey
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
method: searched
name: Orange Business Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Orange Business secures its APIs with apiKey, oauth2, and openIdConnect across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Orange Business
provider_slug: orange-business
scheme_count: 3
schemes:
- description: OpenID Connect authentication
  name: openId
  openIdConnectUrl: https://example.com/.well-known/openid-configuration
  sources:
  - openapi/orange-business-check-device-swap-api-openapi.yml
  - openapi/orange-business-check-sim-swap-api-openapi.yml
  - openapi/orange-business-device-reachability-status-api-openapi.yml
  - openapi/orange-business-geofencing-subscriptions-api-openapi.yml
  - openapi/orange-business-location-retrieval-api-openapi.yml
  - openapi/orange-business-location-verification-api-openapi.yml
  - openapi/orange-business-match-api-openapi.yml
  - openapi/orange-business-phone-number-share-api-openapi.yml
  - openapi/orange-business-phone-number-verify-api-openapi.yml
  - openapi/orange-business-population-density-data-api-openapi.yml
  - openapi/orange-business-qos-sessions-api-openapi.yml
  - openapi/orange-business-retrieve-device-swap-date-api-openapi.yml
  - openapi/orange-business-retrieve-sim-swap-date-api-openapi.yml
  - openapi/orange-business-roaming-status-retrieval-api-openapi.yml
  type: openIdConnect
- in: header
  name: X-API-KEY
  parameter: X-API-KEY
  sources:
  - openapi/orange-business-live-objects-openapi.json
  type: apiKey
- flows:
  - authorizationUrl: https://liveobjects.orange-business.com/api/v1/oauth2/authorize
    flow: authorizationCode
    scopes: 23
    tokenUrl: https://liveobjects.orange-business.com/api/v1/oauth2/token
  name: OAuth2.0
  sources:
  - openapi/orange-business-live-objects-openapi.json
  type: oauth2
slug: orange-business-authentication
source_filename: orange-business-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: searched\nsource: 'openapi/orange-business-check-device-swap-api-openapi.yml, openapi/orange-business-check-sim-swap-api-openapi.yml,\n  openapi/orange-business-device-reachability-status-api-openapi.yml, openapi/orange-business-geofencing-subscriptions-api-openapi.yml,\n  openapi/orange-business-live-objects-openapi.json, openapi/orange-business-location-retrieval-api-openapi.yml,\n  openapi/orange-business-location-verification-api-openapi.yml, openapi/orange-business-match-api-openapi.yml,\n  openapi/orange-business-phone-number-share-api-openapi.yml, openapi/orange-business-phone-number-verify-api-openapi.yml,\n  openapi/orange-business-population-density-data-api-openapi.yml, openapi/orange-business-qos-sessions-api-openapi.yml\n  ... + SEARCHED: the Orange Developer authentication guides (backend-flow, frontend-flow) and the error-handling\n  reference, plus live probes of the token endpoints.'\nsummary:\n  types:\n  - apiKey\n  - oauth2\n\
  \  - openIdConnect\n  api_key_in:\n  - header\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: openId\n  type: openIdConnect\n  openIdConnectUrl: https://example.com/.well-known/openid-configuration\n  description: OpenID Connect authentication\n  sources:\n  - openapi/orange-business-check-device-swap-api-openapi.yml\n  - openapi/orange-business-check-sim-swap-api-openapi.yml\n  - openapi/orange-business-device-reachability-status-api-openapi.yml\n  - openapi/orange-business-geofencing-subscriptions-api-openapi.yml\n  - openapi/orange-business-location-retrieval-api-openapi.yml\n  - openapi/orange-business-location-verification-api-openapi.yml\n  - openapi/orange-business-match-api-openapi.yml\n  - openapi/orange-business-phone-number-share-api-openapi.yml\n  - openapi/orange-business-phone-number-verify-api-openapi.yml\n  - openapi/orange-business-population-density-data-api-openapi.yml\n  - openapi/orange-business-qos-sessions-api-openapi.yml\n  - openapi/orange-business-retrieve-device-swap-date-api-openapi.yml\n\
  \  - openapi/orange-business-retrieve-sim-swap-date-api-openapi.yml\n  - openapi/orange-business-roaming-status-retrieval-api-openapi.yml\n- name: X-API-KEY\n  type: apiKey\n  in: header\n  parameter: X-API-KEY\n  sources:\n  - openapi/orange-business-live-objects-openapi.json\n- name: OAuth2.0\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://liveobjects.orange-business.com/api/v1/oauth2/authorize\n    tokenUrl: https://liveobjects.orange-business.com/api/v1/oauth2/token\n    scopes: 23\n  sources:\n  - openapi/orange-business-live-objects-openapi.json\ndocs:\n- https://docs.developer.orange.com/network-apis/practical-guides/api-authentication/backend-flow\n- https://docs.developer.orange.com/network-apis/practical-guides/api-authentication/frontend-flow\n- https://developer.orange.com/resources/orange-apis-error-handling/\ndocumented:\n  gateway:\n    token_url: https://api.orange.com/oauth/v3/token\n    token_url_probe: POST 2026-08-26 -> 400 {\"\
  error\":\"invalid_request\",\"error_description\":\"Missing grant_type\n      in body\"} (live)\n    playground_token_url: https://api.orange.com/openidconnect/playground/v1.0/token\n    playground_token_url_probe: POST 2026-08-26 -> 415 {\"error\":\"invalid_request\",\"error_description\":\"The\n      URI does not support the requested content type\"} (live)\n    ciba_authorize_url: <authorization server base url>/bc-authorize\n    grants:\n    - client_credentials\n    - urn:openid:params:grant-type:ciba\n    client_auth:\n    - 'Authorization: Basic base64(client_id:client_secret)'\n    - private_key_jwt — client_assertion + client_assertion_type=urn:ietf:params:oauth:client-assertion-type:jwt-bearer,\n      RS256, iss=client_id, exp recommended 5 minutes\n    login_hint: tel:+33712345678\n    scope_form: openid dpv:<dpvValue> <technicalParameter>\n    scope_note: Purpose is bound into the OAuth scope with W3C Data Privacy Vocabulary values — the CAMARA\n      convention for consent-gated\
  \ network data.\n    token_lifetime_seconds: 3600\n    caching: Tokens carry expires_in; Orange documents caching the token and refreshing only on expiry rather\n      than calling /token per request.\n    errors:\n      401 code 40: Missing credentials — missing Authorization header, missing token, or missing Bearer prefix\n      401 code 41: Invalid credentials — invalid, pending or revoked client_id/client_secret\n      401 code 42: Expired credentials — expired OAuth 2.0 token\n      403 code 50: Access denied — API not subscribed, or subscription pending/revoked\n  live_objects:\n    api_key_header: X-API-KEY\n    api_key_note: Keys carry roles (23 named scopes) and a per-key MQTT rate limit; GET /api/v0/apiKeys/current_key\n      introspects the key in use.\n    authorization_url: https://liveobjects.orange-business.com/api/v1/oauth2/authorize\n    token_url: https://liveobjects.orange-business.com/api/v1/oauth2/token\n    refresh_url: https://liveobjects.orange-business.com/api/v1/oauth2/token\n\
  \    flow: authorizationCode\n    scopes: 23\ndiscovery:\n  openid_configuration_reachable: false\n  probes:\n  - url: https://developer.orange.com/.well-known/openid-configuration\n    status: 403\n  - url: https://api.orange.com/.well-known/openid-configuration\n    status: 404\n  - url: https://api.orange.com/.well-known/oauth-authorization-server\n    status: 404\n  - url: https://liveobjects.orange-business.com/.well-known/openid-configuration\n    status: 403\n  note: Every harvested CAMARA contract still declares the upstream placeholder openIdConnectUrl https://example.com/.well-known/openid-configuration.\n    Orange serves no reachable discovery document on any host, so a client cannot resolve the authorization\n    server from the contract — it must be read out of the prose guides.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/orange-business/refs/heads/main/authentication/orange-business-authentication.yml
summary_line: apiKey/oauth2/openIdConnect · 3 schemes
tags:
- 5G
- Artificial Intelligence
- B2B
- CAMARA
- Cloud
- Communications
- Cybersecurity
- Developer Platform
- Digital Workplace
- Enterprise
- France
- IoT
- Identity
- Mobile Money
- Network APIs
- Open Gateway
- Orange
- Payments
- SD-WAN
- SMS
- SASE
- Telco
- Voice
---
