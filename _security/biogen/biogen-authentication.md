---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: biogen-keys-api-openapi.yml
  format: yaml
  label: Biogen Keys API
  slug: biogen-keys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/biogen/refs/heads/main/openapi/biogen-keys-api-openapi.yml
- filename: biogen-services-api-openapi.yml
  format: yaml
  label: Biogen Services API
  slug: biogen-services-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/biogen/refs/heads/main/openapi/biogen-services-api-openapi.yml
- filename: biogen-cdp-export-api-openapi.yml
  format: yaml
  label: Biogen CDP Export API (Non-Production)
  slug: biogen-cdp-export-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/biogen/refs/heads/main/openapi/biogen-cdp-export-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Biogen Authentication
name_suffix: Authentication
oauth_flows: []
overview: Biogen secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Biogen
provider_slug: biogen
scheme_count: 2
schemes:
- description: 'API key issued through the Biogen developer portal, sent on every request. Declared by Biogen''s own published definition as auth.key { param: "x-api-key", location: "header" }.'
  in: header
  name: apiKeyAuth
  parameter: x-api-key
  sources:
  - https://developer1.biogen.com/swagger/export/23683
  - openapi/_original/biogen-cdp-export-api-iodoc.json
  - openapi/biogen-cdp-export-api-openapi.yml
  type: apiKey
- description: Portal-management key form documented for the developer portal's own key and service endpoints. Note the case difference from the gateway's x-api-key — this scheme comes from AE-authored specs transcribed from portal documentation, not from a Biogen-published contract.
  in: header
  name: apiKeyAuth
  parameter: X-API-Key
  sources:
  - openapi/biogen-keys-api-openapi.yml
  - openapi/biogen-services-api-openapi.yml
  type: apiKey
slug: biogen-authentication
source_filename: biogen-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-04'\nmethod: searched\nsource: >-\n  https://developer1.biogen.com/swagger/export/23683 (the provider's own API definition, which\n  declares the auth scheme), https://developer1.biogen.com/io-docs and\n  https://developer.biogen.com/io-docs.\ndocs: https://developer.biogen.com/io-docs\nsummary:\n  types:\n    - apiKey\n  api_key_in:\n    - header\n  oauth2: false\n  mtls: false\nschemes:\n  - name: apiKeyAuth\n    type: apiKey\n    in: header\n    parameter: x-api-key\n    description: >-\n      API key issued through the Biogen developer portal, sent on every request. Declared by Biogen's\n      own published definition as auth.key { param: \"x-api-key\", location: \"header\" }.\n    sources:\n      - https://developer1.biogen.com/swagger/export/23683\n      - openapi/_original/biogen-cdp-export-api-iodoc.json\n      - openapi/biogen-cdp-export-api-openapi.yml\n  - name: apiKeyAuth\n    type: apiKey\n    in: header\n    parameter: X-API-Key\n    description:\
  \ >-\n      Portal-management key form documented for the developer portal's own key and service\n      endpoints. Note the case difference from the gateway's x-api-key — this scheme comes from\n      AE-authored specs transcribed from portal documentation, not from a Biogen-published contract.\n    sources:\n      - openapi/biogen-keys-api-openapi.yml\n      - openapi/biogen-services-api-openapi.yml\nissuance:\n  self_service: false\n  flow: >-\n    Keys are requested through the portal's \"Request Access Key\" / Manage Keys screens, which require\n    a portal account. Registration is not open: the portal's Register link carries an empty href and\n    the portal stylesheet hides the register control, with sign-in handled by external SSO\n    (https://developer.biogen.com/login/external). Access is therefore employee/partner-issued.\noauth2:\n  declared: false\n  note: >-\n    The Mashery/Boomi io-docs page renders an OAuth 2.0 flow selector (authorization code, client\n    credentials,\
  \ password, implicit) for every portal it hosts. That is platform chrome, not a Biogen\n    claim — the one Biogen API definition readable anonymously declares data-auth-type=\"key\". No\n    OAuth2 scheme is asserted here and no scopes/ artifact is written.\ntransport:\n  https_only: true\n  evidence: >-\n    Biogen portal reference: the API \"strictly uses HTTPS in the transport layer\". TLS confirmed live\n    on every host (security/biogen-domain-security.yml).\ndiscovery:\n  openid_configuration: false\n  oauth_authorization_server: false\n  protected_resource_metadata: false\n  evidence: well-known/biogen-well-known.yml — all five named paths missed on all six hosts.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/biogen/refs/heads/main/authentication/biogen-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Biotechnology
- Healthcare
- Life Sciences
- Pharmaceuticals
- Neurology
- Fortune 500
---
