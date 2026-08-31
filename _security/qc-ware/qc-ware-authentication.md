---
api_key_in: []
api_specs:
- filename: qc-ware-files-api-openapi.yml
  format: yaml
  label: QC Ware Files API
  slug: qc-ware-files-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qc-ware/refs/heads/main/openapi/qc-ware-files-api-openapi.yml
- filename: qc-ware-workflows-api-openapi.yml
  format: yaml
  label: QC Ware Workflows API
  slug: qc-ware-workflows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qc-ware/refs/heads/main/openapi/qc-ware-workflows-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
method: searched
name: Qc Ware Authentication
name_suffix: Authentication
oauth_flows: []
overview: QC Ware declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: QC Ware
provider_slug: qc-ware
scheme_count: 0
schemes: []
slug: qc-ware-authentication
source_filename: qc-ware-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: searched\nsource: https://github.com/qcware/promethium-examples/blob/main/examples/Getting_Started/01_Single_Point_Calculation/cURL/cURL.md\ndocs: https://app.promethium.qcware.com/settings/\nnote: >-\n  The published OpenAPI declares NO components.securitySchemes. Authentication is instead modelled as a\n  REQUIRED header parameter named X-API-KEY on every one of the 13 operations — a FastAPI-generated spec\n  shape. The scheme below is therefore recorded from the provider's own cURL example and CLI documentation\n  rather than derived from a securityScheme block, which is why method is `searched` and not `derived`.\napis:\n- name: Promethium REST API\n  baseURL: https://api.promethium.qcware.com\n  spec: openapi/qc-ware-promethium-openapi.yml\n  schemes:\n  - id: promethium-api-key\n    type: apiKey\n    in: header\n    name: X-API-KEY\n    required: true\n    applied_to: all 13 operations (declared as a required header parameter, not a securityScheme)\n\
  \    description: >-\n      A per-account Promethium API key. Created from the API tab of the Promethium settings page at\n      https://app.promethium.qcware.com/settings/. Sent verbatim in the X-API-Key request header.\n      The provider's cURL example uses the placeholder PM_API_KEY.\n    key_prefix: null\n    key_prefix_note: The provider does not publish a documented key prefix.\n    rotation: not documented\n    storage:\n      cli: >-\n        `pm config credentials` prompts for the key and writes it to a `.promethium.ini` file in the\n        user's home directory; the Python SDK (PromethiumClient) reads the same file.\n      env_var: not documented\n  identity_sources:\n    note: >-\n      The spec's AuthSource enum names the two identity paths Promethium itself recognises.\n    values:\n    - id: api_key\n      description: Programmatic access via the X-API-Key header (the REST API and SDK/CLI path).\n    - id: auth0\n      description: >-\n        Interactive console sign-in.\
  \ QC Ware's web properties link to an Auth0 universal-login tenant at\n        qcs.us.auth0.com. This is the human console path; it is NOT exposed as an OAuth surface for the\n        public REST API, and no OAuth authorization/token endpoint is published.\n  oauth2: false\n  openid_connect: false\n  mutual_tls: false\n  scopes:\n    published: false\n    note: >-\n      No OAuth2 flows and no scope/permission reference are published, so no scopes/ artifact is emitted.\n      Access is all-or-nothing on a single account-scoped API key.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/qc-ware/refs/heads/main/authentication/qc-ware-authentication.yml
summary_line: 0 schemes
tags:
- Company
- Quantum Computing
- Computational Chemistry
- Quantum Chemistry
- Drug Discovery
- Materials Science
- Scientific Computing
- GPU Computing
- Life Sciences
- Simulation
---
