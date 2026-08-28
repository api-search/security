---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: searched
name: Sight Machine Authentication
name_suffix: Authentication
oauth_flows: []
overview: Sight Machine declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: Sight Machine
provider_slug: sight-machine
scheme_count: 3
schemes:
- description: The primary programmatic credential. A key id and its matching secret are generated inside the tenant UI under Settings > Profile > Security, and both are sent as separate request headers on every call. This is the credential used by the Dashboard API, by the SDK's apikey login mode, and by the ODBC/JDBC connector (where the key is the username and the secret is the password).
  id: api-key-pair
  in: header
  names:
  - X-SM-API-Key-Id
  - X-SM-API-Secret
  provisioning: https://docs.sightmachine.com/docs/apis
  scope: tenant
  type: apiKey
- description: Interactive email + password login, exposed by the SDK as cli.login('basic', email=..., password=...). Establishes a session cookie against the tenant host. Intended for human/notebook use, not for automation.
  id: basic-login
  scheme: basic
  scope: tenant
  type: http
- description: A separate class of key, called an Edge API key, minted under CONNECT in the platform UI and used to authenticate FactoryTX edge collectors uploading raw plant data into the tenant. Distinct from the Dashboard/SDK key pair — it authorises ingestion, not query.
  id: edge-api-key
  in: header
  provisioning: https://docs.sightmachine.com/docs/apis
  scope: tenant-ingestion
  type: apiKey
slug: sight-machine-authentication
source_filename: sight-machine-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-27'\nmethod: searched\nsource: https://docs.sightmachine.com/docs/apis\ndocs: https://docs.sightmachine.com/docs/apis\nnote: >-\n  Derived from the provider's own API and SDK documentation and confirmed against the\n  live tenant host. There is no OpenAPI to derive securitySchemes from, so this profile\n  was written from the docs and from the first-party SDK's login implementation.\n  Unauthenticated requests to https://demo.sightmachine.io/v1/datatab/cycle were observed\n  returning HTTP 401 with {\"error\":\"unauthenticated\"} on 2026-08-27.\nschemes:\n- id: api-key-pair\n  type: apiKey\n  in: header\n  names:\n  - X-SM-API-Key-Id\n  - X-SM-API-Secret\n  description: >-\n    The primary programmatic credential. A key id and its matching secret are generated\n    inside the tenant UI under Settings > Profile > Security, and both are sent as\n    separate request headers on every call. This is the credential used by the Dashboard\n    API, by the SDK's\
  \ apikey login mode, and by the ODBC/JDBC connector (where the key\n    is the username and the secret is the password).\n  provisioning: https://docs.sightmachine.com/docs/apis\n  scope: tenant\n- id: basic-login\n  type: http\n  scheme: basic\n  description: >-\n    Interactive email + password login, exposed by the SDK as\n    cli.login('basic', email=..., password=...). Establishes a session cookie against the\n    tenant host. Intended for human/notebook use, not for automation.\n  scope: tenant\n- id: edge-api-key\n  type: apiKey\n  in: header\n  description: >-\n    A separate class of key, called an Edge API key, minted under CONNECT in the platform\n    UI and used to authenticate FactoryTX edge collectors uploading raw plant data into\n    the tenant. Distinct from the Dashboard/SDK key pair — it authorises ingestion, not\n    query.\n  provisioning: https://docs.sightmachine.com/docs/apis\n  scope: tenant-ingestion\noauth2: false\nopenid_connect: false\nmutual_tls: false\nobservations:\n\
  - url: https://demo.sightmachine.io/v1/datatab/cycle\n  status: 401\n  body: '{\"description\":\"Not logged in or invalid API key provided\",\"details\":{},\"error\":\"unauthenticated\"}'\n- url: https://demo.sightmachine.io/v1/obj/dashboard/1/full_values\n  status: 401\n  body: '{\"description\":\"Not logged in or invalid API key provided\",\"details\":{},\"error\":\"unauthenticated\"}'\n- url: https://demo.sightmachine.io/.well-known/openid-configuration\n  status: 404\n- url: https://demo.sightmachine.io/.well-known/oauth-authorization-server\n  status: 404\ngaps:\n- >-\n  No OAuth 2.0, no OpenID Connect discovery document and no published scope model —\n  credentials are tenant-wide key pairs with no documented least-privilege granularity.\n- >-\n  Key rotation and expiry policy is not documented on any public page.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sight-machine/refs/heads/main/authentication/sight-machine-authentication.yml
summary_line: 3 schemes
tags:
- Manufacturing
- Industrial IoT
- Analytics
- Artificial Intelligence
- Agents
- Data
- OPC UA
- MQTT
- Digital Twin
- Operations
---
