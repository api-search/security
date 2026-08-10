---
api_key_in:
- header
api_specs:
- filename: disqo-audience-api-postman.json
  format: json
  label: DISQO Audience Projects API
  slug: disqo-audience-projects-api
  spec_type: Postman
  url: https://raw.githubusercontent.com/api-evangelist/disqo/refs/heads/main/postman/disqo-audience-api-postman.json
auth_types:
- http
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Disqo Authentication
name_suffix: Authentication
oauth_flows: []
overview: DISQO secures its APIs with http and apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: DISQO
provider_slug: disqo
scheme_count: 2
schemes:
- applies_to:
  - https://projects-api.audience.disqo.com
  - https://feasibility-api.audience.disqo.com
  - https://custom-questions-api.audience.disqo.com
  credentials:
    password: API key
    username: clientId
  encoding: echo -n {clientId}:{apiKey} | base64
  header: 'Authorization: Basic {base64(clientId:apiKey)}'
  name: audienceBasicAuth
  provisioning: Credentials are issued by DISQO during onboarding; the demo/sandbox environment uses a separate credential pair requested from the integration contact. There is no self-service key issuance.
  scheme: basic
  source: https://developer.disqo.com/docs/audience-api/
  type: http
- applies_to:
  - https://coreg.us.sjapis.com/api
  in: header
  name: coregApiKey
  name_param: Authorization
  provisioning: '"An API Key will be provided to use the API. If one has not been provided, contact your Account Manager."'
  source: https://developer.disqo.com/docs/coreg-api/
  type: apiKey
  value_format: ApiKey {uniqueApiKey}
slug: disqo-authentication
source_filename: disqo-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-04'\nmethod: searched\nsource: https://developer.disqo.com/docs/audience-api/\ndocs:\n- https://developer.disqo.com/docs/audience-api/\n- https://developer.disqo.com/docs/coreg-api/\nsummary:\n  types: [http, apiKey]\n  http_schemes: [basic]\n  api_key_in: [header]\n  oauth2_flows: []\n  oauth2: false\n  openid_connect: false\n  mutual_tls: false\n  note: >-\n    DISQO uses no OAuth 2.0 and no OpenID Connect on any public API. The Audience\n    API family is HTTP Basic (clientId as username, API key as password); the\n    CoReg API is a bearer-style ApiKey header. There is therefore no scope\n    surface — scopes/ is intentionally not emitted for this provider.\nschemes:\n- name: audienceBasicAuth\n  type: http\n  scheme: basic\n  applies_to:\n  - https://projects-api.audience.disqo.com\n  - https://feasibility-api.audience.disqo.com\n  - https://custom-questions-api.audience.disqo.com\n  credentials:\n    username: clientId\n    password: API key\n  header:\
  \ 'Authorization: Basic {base64(clientId:apiKey)}'\n  encoding: 'echo -n {clientId}:{apiKey} | base64'\n  provisioning: >-\n    Credentials are issued by DISQO during onboarding; the demo/sandbox\n    environment uses a separate credential pair requested from the integration\n    contact. There is no self-service key issuance.\n  source: https://developer.disqo.com/docs/audience-api/\n- name: coregApiKey\n  type: apiKey\n  in: header\n  name_param: Authorization\n  value_format: 'ApiKey {uniqueApiKey}'\n  applies_to:\n  - https://coreg.us.sjapis.com/api\n  provisioning: >-\n    \"An API Key will be provided to use the API. If one has not been provided,\n    contact your Account Manager.\"\n  source: https://developer.disqo.com/docs/coreg-api/\nmessage_authentication:\n- name: callbackHmac\n  purpose: >-\n    Integrity of the panelist redirect/callback. Every parameter on the callback\n    URL preceding &auth is signed and the signature is appended as auth.\n  algorithm: HMAC-SHA256\n \
  \ encoding: base64url, unpadded (URL-safe, no padding)\n  key: shared secret key issued by DISQO\n  applies_to:\n  - https://go.audience.disqo.com/callback/\n  - https://go.audience.disqo-demo.com/callback/\n  source: https://developer.disqo.com/docs/audience-api/\ntransport:\n  https_required: true\n  tls_observed: TLSv1.3\n  source: security/disqo-domain-security.yml\ngaps_to_push_back_to_provider:\n- >-\n  HTTP Basic with a long-lived shared secret is the only client authentication\n  offered. There is no OAuth 2.0 client-credentials flow, no key rotation\n  endpoint, and no documented key-expiry policy — all of which an agent or a\n  multi-tenant integrator needs.\n- >-\n  No machine-readable declaration of these schemes exists (no OpenAPI\n  securitySchemes), so the auth contract can only be read by a human from the\n  Slate docs.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/disqo/refs/heads/main/authentication/disqo-authentication.yml
summary_line: http/apiKey · 2 schemes
tags:
- Company
- Audience
- Market Research
- Surveys
- Consumer Insights
- Advertising Measurement
- Panel
- Brand Lift
- Data
- Analytics
---
