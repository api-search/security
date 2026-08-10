---
api_key_in: []
api_specs:
- filename: alice--bob-health-api-openapi.yml
  format: yaml
  label: Alice Bob Health API
  slug: alice--bob-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alice--bob/refs/heads/main/openapi/alice--bob-health-api-openapi.yml
- filename: alice--bob-jobs-api-openapi.yml
  format: yaml
  label: Alice Bob Jobs API
  slug: alice--bob-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alice--bob/refs/heads/main/openapi/alice--bob-jobs-api-openapi.yml
- filename: alice--bob-targets-api-openapi.yml
  format: yaml
  label: Alice Bob Targets API
  slug: alice--bob-targets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alice--bob/refs/heads/main/openapi/alice--bob-targets-api-openapi.yml
auth_types: []
description: Felis Cloud uses a single static API key. There is no OAuth, no OIDC, no JWT, no mTLS and no scope model. This artifact is method `searched` rather than `derived` because the published OpenAPI declares an EMPTY components.securitySchemes and models the credential as an OPTIONAL `authorization` header parameter — deriving from the spec alone would say the API is unauthenticated, which is wrong.
kind: authentication
layout: security
method: searched
name: Alice  Bob Authentication
name_suffix: Authentication
oauth_flows: []
overview: Alice Bob declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Alice Bob
provider_slug: alice--bob
scheme_count: 1
schemes:
- encoding: none
  example_shape: 'Authorization: Basic <API key>'
  id: apiKeyAuth
  in: header
  name: Authorization
  note: 'The literal token `Basic` is followed by the RAW API key. This is NOT RFC 7617 HTTP Basic authentication — the key is not base64-encoded and there is no user:password pair. Sending genuine RFC 7617 credentials will fail. Confirmed both in the docs curl example and in ApiClient.__init__, which sets `self._session.headers.update({''Authorization'': f''Basic {api_key}''})`.'
  required: true
  sources:
  - https://felis.alice-bob.com/docs/reference/the_api/
  - https://github.com/Alice-Bob-SW/qiskit-alice-bob-provider
  type: apiKey
  value_format: Basic <API key>
slug: alice--bob-authentication
source_filename: alice--bob-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-06'\nmethod: searched\nsource: >-\n  https://felis.alice-bob.com/docs/reference/the_api/ (the published curl example),\n  https://felis.alice-bob.com/docs/felis_cloud/connect_to_felis_cloud/ (key issuance), and the\n  reference client\n  https://github.com/Alice-Bob-SW/qiskit-alice-bob-provider/blob/main/qiskit_alice_bob_provider/remote/api/client.py\n  (the exact header it sets). Live behaviour confirmed by probing\n  https://api-gcp.alice-bob.com/v1/health/ unauthenticated on 2026-08-06 (401).\ndocs: https://felis.alice-bob.com/docs/felis_cloud/connect_to_felis_cloud/\ndescription: >-\n  Felis Cloud uses a single static API key. There is no OAuth, no OIDC, no JWT, no mTLS and no\n  scope model. This artifact is method `searched` rather than `derived` because the published\n  OpenAPI declares an EMPTY components.securitySchemes and models the credential as an\n  OPTIONAL `authorization` header parameter — deriving from the spec alone would say the API\n\
  \  is unauthenticated, which is wrong.\n\nderived_from_spec: false\nspec_declares_security_schemes: false\nspec_gap: >-\n  openapi/alice--bob-felis-cloud-openapi.json has no components.securitySchemes and no root\n  `security` requirement. 12 of its 14 operations declare `authorization` as an optional\n  (`anyOf: [string, null]`) header parameter; list_targets and target availabilities declare no\n  auth parameter at all. In reality the host is authenticated by default: every path, including\n  /.well-known/*, returns 401 without a key. Corrected in\n  overlays/alice--bob-felis-cloud-overlay.yaml.\n\nschemes:\n  - id: apiKeyAuth\n    type: apiKey\n    in: header\n    name: Authorization\n    value_format: 'Basic <API key>'\n    required: true\n    encoding: none\n    note: >-\n      The literal token `Basic` is followed by the RAW API key. This is NOT RFC 7617 HTTP Basic\n      authentication — the key is not base64-encoded and there is no user:password pair. Sending\n      genuine RFC\
  \ 7617 credentials will fail. Confirmed both in the docs curl example and in\n      ApiClient.__init__, which sets\n      `self._session.headers.update({'Authorization': f'Basic {api_key}'})`.\n    example_shape: 'Authorization: Basic <API key>'\n    sources:\n      - https://felis.alice-bob.com/docs/reference/the_api/\n      - https://github.com/Alice-Bob-SW/qiskit-alice-bob-provider\n\nkey_management:\n  issuance_url: https://api-gcp.alice-bob.com/console/\n  issuance_path: '\"API KEYS\" tab in the Felis Cloud console'\n  identity_provider: >-\n    Google account — the console is entered with the Google account used to subscribe to Felis\n    Cloud on Google Cloud Marketplace.\n  prerequisite: An active Felis Cloud subscription via https://console.cloud.google.com/marketplace/product/cloud-prod-0/felis-cloud\n  rotation: >-\n    Keys are created and revoked in the console. The docs recommend one key per person so that\n    billing can be attributed and access revoked individually.\n\
  \  expiry: not documented\n  scopes: none — the key is all-or-nothing across the whole API\n\ntenancy:\n  model: implicit\n  note: >-\n    There is no account, organisation or project resource in the API. Tenancy is carried by the\n    key and surfaces only as the denormalised `userId`, `userName` and `organizationName`\n    strings on ExternalJob. GET /v1/jobs/ is documented as returning \"all active and completed\n    jobs associated with the authenticated user\".\n\nnot_supported:\n  oauth2: true\n  openid_connect: true\n  mutual_tls: true\n  bearer_jwt: true\n  hmac_request_signing: true\n  webhook_signature_verification: 'n/a — no webhook surface exists'\n\nfailure_mode:\n  status: 401\n  body: '{\"error\": {\"code\": 401, \"message\": \"Unauthorized\"}}'\n  scope: every path on api-gcp.alice-bob.com and api.alice-bob.com\n  exceptions: [/openapi.json, /reference, /console/*]\n  detail: errors/alice--bob-problem-types.yml\n\ntransport_security:\n  https_required: true\n  detail: security/alice--bob-domain-security.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/alice--bob/refs/heads/main/authentication/alice--bob-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Quantum Computing
- Quantum
- Cloud Computing
- Emulation
- Developer Tools
- Compute
- Hardware
- Research
- Qiskit
- QIR
---
