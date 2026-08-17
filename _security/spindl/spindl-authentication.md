---
api_key_in:
- header
api_specs:
- filename: spindl-events-api-openapi.yml
  format: yaml
  label: Spindl Events API
  slug: spindl-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spindl/refs/heads/main/openapi/spindl-events-api-openapi.yml
- filename: spindl-short-links-api-openapi.yml
  format: yaml
  label: Spindl Short Links API
  slug: spindl-short-links-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spindl/refs/heads/main/openapi/spindl-short-links-api-openapi.yml
- filename: spindl-ads-api-openapi.yml
  format: yaml
  label: Spindl Ads API
  slug: spindl-ads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spindl/refs/heads/main/openapi/spindl-ads-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Spindl Authentication
name_suffix: Authentication
oauth_flows: []
overview: Spindl secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Spindl
provider_slug: spindl
scheme_count: 2
schemes:
- description: Publisher API Token generated on the Settings screen in the Spindl app. Distinct from the Server-to-Server X-API-Key and from the client-side SDK key. Must be treated as a secret and never shipped in public-facing code.
  in: header
  name: PublisherApiKey
  parameter: X-API-ACCESS-KEY
  sources:
  - openapi/spindl-ads-api-openapi.yml
  type: apiKey
- description: Server-to-Server API key generated on the Settings page in the Spindl app (https://app.spindl.xyz/settings). Distinct from the client-side SDK key.
  in: header
  name: ApiKeyAuth
  parameter: X-API-Key
  sources:
  - openapi/spindl-events-api-openapi.yml
  - openapi/spindl-short-links-api-openapi.yml
  type: apiKey
slug: spindl-authentication
source_filename: spindl-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: openapi/spindl-ads-api-openapi.yml, openapi/spindl-events-api-openapi.yml, openapi/spindl-short-links-api-openapi.yml\ndocs: https://docs.spindl.xyz/technical/api\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  credential_count: 3\n  note: >-\n    Spindl issues THREE distinct credentials, all from the Settings screen of\n    the Spindl app, and they are not interchangeable: the Server-to-Server API\n    key (X-API-Key), the Publisher API Token (X-API-ACCESS-KEY) for the Ads\n    API, and the client-side SDK Key used by the browser and mobile SDKs. Only\n    the first two are HTTP request credentials and appear in schemes[] below.\n    Server keys are revocable from Settings by clicking the X beside the token.\n    No OAuth2, OIDC or mutualTLS is offered — /.well-known/openid-configuration\n    and /.well-known/oauth-authorization-server miss on every host, so no\n    scopes/ artifact is emitted.\nclient_credentials:\n\
  - name: SDK Key\n  used_by: [browser JS SDK, HTML script tag, Android SDK, iOS SDK]\n  transport: >-\n    Config value (`sdkKey`) or `data-key` script attribute — not an HTTP header\n  public: true\n  docs: https://docs.spindl.xyz/technical/javascript-sdk-html-script-guide/install\n  note: >-\n    Public by nature since it ships in client code. Spindl's hardening guidance\n    for it is version pinning and Subresource Integrity rather than secrecy —\n    see https://docs.spindl.xyz/technical/javascript-sdk-html-script-guide/security\nschemes:\n- name: PublisherApiKey\n  type: apiKey\n  in: header\n  parameter: X-API-ACCESS-KEY\n  description: Publisher API Token generated on the Settings screen in the Spindl app. Distinct\n    from the Server-to-Server X-API-Key and from the client-side SDK key. Must be treated as\n    a secret and never shipped in public-facing code.\n  sources:\n  - openapi/spindl-ads-api-openapi.yml\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n\
  \  description: Server-to-Server API key generated on the Settings page in the Spindl app (https://app.spindl.xyz/settings).\n    Distinct from the client-side SDK key.\n  sources:\n  - openapi/spindl-events-api-openapi.yml\n  - openapi/spindl-short-links-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/spindl/refs/heads/main/authentication/spindl-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Company
- Crypto Web3
- Attribution
- Analytics
- Marketing
- Growth
- SDK
- Web3
---
