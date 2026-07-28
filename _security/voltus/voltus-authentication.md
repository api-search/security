---
api_key_in:
- header
api_specs:
- filename: voltus-openapi.yml
  format: yaml
  label: Voltus Dispatches API
  slug: voltus-dispatches-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/voltus/refs/heads/main/openapi/voltus-openapi.yml
- filename: voltus-openapi.yml
  format: yaml
  label: Voltus Sites API
  slug: voltus-sites-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/voltus/refs/heads/main/openapi/voltus-openapi.yml
- filename: voltus-openapi.yml
  format: yaml
  label: Voltus Telemetry API
  slug: voltus-telemetry-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/voltus/refs/heads/main/openapi/voltus-openapi.yml
- filename: voltus-openapi.yml
  format: yaml
  label: Voltus Webhooks API
  slug: voltus-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/voltus/refs/heads/main/openapi/voltus-openapi.yml
auth_types:
- apiKey
- mutualTLS
description: Voltus authenticates the REST API with a single static API key in a custom header, and the OpenADR 2.0a VTN with mutual TLS. There is no OAuth, no OpenID Connect, no scopes and no self-serve key issuance - keys come from a Voltus account manager and are entitled to specific sites. A public sandbox key is published in the docs and works, anonymously, against sandbox.voltus.co only.
kind: authentication
layout: security
method: searched
name: Voltus Authentication
name_suffix: Authentication
oauth_flows: []
overview: Voltus secures its APIs with apiKey and mutualTLS across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Voltus
provider_slug: voltus
scheme_count: 2
schemes:
- description: '"The API uses API key authentication. API keys are provided by your account manager. Each request must include an X-Voltus-API-Key header where the value is your API key." Applied globally - every one of the ten published operations also declares X-Voltus-API-Key as a required header parameter.'
  docs: https://api.voltus.co/docs/openapi/voltus-api-reference
  environments:
  - base_url: https://api.voltus.co/2022-04-15
    key: issued by Voltus
    name: production
  - base_url: https://sandbox.voltus.co/2022-04-15
    key: secret
    name: sandbox-public
    published: true
    published_at: https://api.voltus.co/docs/concepts/public-credentials
  - base_url: https://sandbox.voltus.co/2022-04-15
    key: issued by Voltus
    name: sandbox-keyed
    note: required for the POST /scenarios dispatch simulations
  in: header
  issuance: Voltus account manager, after a commercial agreement.
  name: X-Voltus-API-Key
  parameter: X-Voltus-API-Key
  scoping: Production keys are configured for specific sites; contact Voltus support to add or remove sites from a key.
  sources:
  - openapi/voltus-openapi.yml
  type: apiKey
- description: The OpenADR 2.0a VTN authenticates VENs with mutual TLS. The partner emails an X.509 Certificate Signing Request to api-support@voltus.co with Common Name YOUR_VEN_ID@openadr.voltus.co; Voltus returns a signed client certificate (encrypted zip plus a one-time password link) that the VEN presents on every request.
  docs: https://api.voltus.co/docs/concepts/openadr
  endpoints:
  - https://openadr.voltus.co/vtn/YOUR_VEN_ID/OpenADR2/Simple/EiEvent
  - https://openadr-sandbox.voltus.co/vtn/YOUR_VEN_ID/OpenADR2/Simple/EiEvent
  name: OpenADR mutual TLS
  sources:
  - https://api.voltus.co/docs/tutorials/openadr
  type: mutualTLS
slug: voltus-authentication
source_filename: voltus-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-27'\nmethod: searched\nsource: openapi/voltus-openapi.yml\ndocs: https://api.voltus.co/docs/openapi/voltus-api-reference\ndescription: >-\n  Voltus authenticates the REST API with a single static API key in a custom\n  header, and the OpenADR 2.0a VTN with mutual TLS. There is no OAuth, no OpenID\n  Connect, no scopes and no self-serve key issuance - keys come from a Voltus\n  account manager and are entitled to specific sites. A public sandbox key is\n  published in the docs and works, anonymously, against sandbox.voltus.co only.\nsummary:\n  types:\n  - apiKey\n  - mutualTLS\n  api_key_in:\n  - header\n  oauth2_flows: []\n  scopes: none\nschemes:\n- name: X-Voltus-API-Key\n  type: apiKey\n  in: header\n  parameter: X-Voltus-API-Key\n  sources:\n  - openapi/voltus-openapi.yml\n  docs: https://api.voltus.co/docs/openapi/voltus-api-reference\n  description: >-\n    \"The API uses API key authentication. API keys are provided by your account\n    manager.\
  \ Each request must include an X-Voltus-API-Key header where the value\n    is your API key.\" Applied globally - every one of the ten published\n    operations also declares X-Voltus-API-Key as a required header parameter.\n  issuance: Voltus account manager, after a commercial agreement.\n  scoping: >-\n    Production keys are configured for specific sites; contact Voltus support to\n    add or remove sites from a key.\n  environments:\n  - {name: production, base_url: 'https://api.voltus.co/2022-04-15', key: issued by Voltus}\n  - {name: sandbox-public, base_url: 'https://sandbox.voltus.co/2022-04-15', key: secret, published: true, published_at: 'https://api.voltus.co/docs/concepts/public-credentials'}\n  - {name: sandbox-keyed, base_url: 'https://sandbox.voltus.co/2022-04-15', key: issued by Voltus, note: 'required for the POST /scenarios dispatch simulations'}\n- name: OpenADR mutual TLS\n  type: mutualTLS\n  sources:\n  - https://api.voltus.co/docs/tutorials/openadr\n  docs: https://api.voltus.co/docs/concepts/openadr\n\
  \  description: >-\n    The OpenADR 2.0a VTN authenticates VENs with mutual TLS. The partner emails\n    an X.509 Certificate Signing Request to api-support@voltus.co with Common\n    Name YOUR_VEN_ID@openadr.voltus.co; Voltus returns a signed client\n    certificate (encrypted zip plus a one-time password link) that the VEN\n    presents on every request.\n  endpoints:\n  - https://openadr.voltus.co/vtn/YOUR_VEN_ID/OpenADR2/Simple/EiEvent\n  - https://openadr-sandbox.voltus.co/vtn/YOUR_VEN_ID/OpenADR2/Simple/EiEvent\nremoved_schemes:\n- name: 'Authorization: Bearer'\n  removed_in: '2022-04-15'\n  replacement: X-Voltus-API-Key header\n  source: https://api.voltus.co/docs/openapi/voltus-api-reference\nnot_supported:\n  oauth2: true\n  openid_connect: true\n  scopes: true\n  evidence: >-\n    https://voltus.co/.well-known/openid-configuration and\n    https://api.voltus.co/.well-known/openid-configuration both return 404, and\n    /.well-known/oauth-authorization-server returns 404 (probed\
  \ 2026-07-27).\n    No scopes or permissions reference page exists, so no scopes/ artifact is emitted.\nfailure_modes:\n- {status: 400, meaning: header absent, body: '{\"message\":\"\\\"X-Voltus-API-Key\\\" is missing from header\",\"type\":\"Bad Request\"}'}\n- {status: 401, meaning: 'key not entitled - what production returns to the public sandbox key', body: '{\"message\":\"Permission denied\",\"type\":\"Unauthorized\"}'}\n- {status: 403, meaning: 'declared in the spec as \"Unauthorized: Forbidden response.\"'}\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/voltus/refs/heads/main/authentication/voltus-authentication.yml
summary_line: apiKey/mutualTLS · 2 schemes
tags:
- Energy
- United States
- Electricity
- Demand Response
- Virtual Power Plant
- DER
- Grid
- Energy Markets
- Flexibility
- Energy Storage
- OpenADR
- Telemetry
---
