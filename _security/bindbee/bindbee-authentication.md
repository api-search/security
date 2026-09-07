---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: bindbee-candidates-api-openapi.yml
  format: yaml
  label: Bindbee Candidates API
  slug: bindbee-candidates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bindbee/refs/heads/main/openapi/bindbee-candidates-api-openapi.yml
- filename: bindbee-departments-api-openapi.yml
  format: yaml
  label: Bindbee Departments API
  slug: bindbee-departments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bindbee/refs/heads/main/openapi/bindbee-departments-api-openapi.yml
- filename: bindbee-employees-api-openapi.yml
  format: yaml
  label: Bindbee Employees API
  slug: bindbee-employees-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bindbee/refs/heads/main/openapi/bindbee-employees-api-openapi.yml
- filename: bindbee-jobs-api-openapi.yml
  format: yaml
  label: Bindbee Jobs API
  slug: bindbee-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bindbee/refs/heads/main/openapi/bindbee-jobs-api-openapi.yml
- filename: bindbee-time-off-api-openapi.yml
  format: yaml
  label: Bindbee Time Off API
  slug: bindbee-time-off-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bindbee/refs/heads/main/openapi/bindbee-time-off-api-openapi.yml
- filename: bindbee-unified-api-openapi.json
  format: json
  label: Bindbee Unified API
  slug: bindbee-unified-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bindbee/refs/heads/main/openapi/bindbee-unified-api-openapi.json
auth_types:
- http
- apiKey
description: Bindbee authenticates in two layers that are used together, not alternately. The API key identifies the CUSTOMER (and picks the environment); the connector token identifies WHICH OF THEIR END USERS' data is being touched. Only the first is declared in the OpenAPI as a security scheme.
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Bindbee Authentication
name_suffix: Authentication
oauth_flows: []
overview: Bindbee secures its APIs with http and apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Bindbee
provider_slug: bindbee
scheme_count: 2
schemes:
- applied_to_operations: 144
  declared_in_spec: true
  description: The Bindbee API key. Required on every request. Issued and regenerated in the dashboard at https://app.bindbee.dev/settings/keys.
  format: Bearer <BINDBEE_API_KEY>
  in: header
  name: HTTPBearer
  parameter: Authorization
  scheme: bearer
  scope: organization
  sources:
  - openapi/_original/bindbee-openapi.json
  - https://docs.bindbee.dev/api-reference/basics/authentication
  type: http
- declared_in_spec: false
  declared_in_spec_note: NOT declared as a securityScheme. It appears on operations as an ordinary header parameter, so generated clients and security tooling do not treat it as a credential. This is the single most consequential gap in the contract's auth description, and overlays/bindbee-unified-api-overlay.yaml declares it.
  description: Per-end-customer token authorizing access to that customer's HR data. Obtained by running the Bindbee Embed / Magic Link flow and exchanging the returned temporary_token at GET /api/embedded/v1/connectors/connector_token/{temporary_token}. Rate limits are counted against this token.
  format: <connector_token>
  in: header
  name: ConnectorToken
  parameter: X-Connector-Token
  required_on: every operation that reads or writes an end user's data. Organization-level operations (connector list, custom-field configuration, webhook and log reads, integration lookup) take the API key alone.
  scope: end customer
  sources:
  - https://docs.bindbee.dev/api-reference/basics/authentication
  - https://docs.bindbee.dev/sdk/get-connector-token
  type: apiKey
slug: bindbee-authentication
source_filename: bindbee-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-04'\nmethod: searched\nsource: >-\n  https://docs.bindbee.dev/api-reference/basics/authentication,\n  https://docs.bindbee.dev/features/environments/development,\n  https://docs.bindbee.dev/features/environments/production, and\n  openapi/_original/bindbee-openapi.json\ndocs: https://docs.bindbee.dev/api-reference/basics/authentication\nprovider: Bindbee\nproviderId: bindbee\ndescription: >-\n  Bindbee authenticates in two layers that are used together, not alternately. The API key\n  identifies the CUSTOMER (and picks the environment); the connector token identifies WHICH OF\n  THEIR END USERS' data is being touched. Only the first is declared in the OpenAPI as a security\n  scheme.\nsummary:\n  types:\n  - http\n  - apiKey\n  oauth2: false\n  openIdConnect: false\n  mutualTLS: false\n  api_key_in:\n  - header\nschemes:\n- name: HTTPBearer\n  type: http\n  scheme: bearer\n  in: header\n  parameter: Authorization\n  format: 'Bearer <BINDBEE_API_KEY>'\n \
  \ scope: organization\n  declared_in_spec: true\n  applied_to_operations: 144\n  description: >-\n    The Bindbee API key. Required on every request. Issued and regenerated in the dashboard at\n    https://app.bindbee.dev/settings/keys.\n  sources:\n  - openapi/_original/bindbee-openapi.json\n  - https://docs.bindbee.dev/api-reference/basics/authentication\n- name: ConnectorToken\n  type: apiKey\n  in: header\n  parameter: X-Connector-Token\n  format: '<connector_token>'\n  scope: end customer\n  declared_in_spec: false\n  declared_in_spec_note: >-\n    NOT declared as a securityScheme. It appears on operations as an ordinary header parameter, so\n    generated clients and security tooling do not treat it as a credential. This is the single\n    most consequential gap in the contract's auth description, and\n    overlays/bindbee-unified-api-overlay.yaml declares it.\n  description: >-\n    Per-end-customer token authorizing access to that customer's HR data. Obtained by running the\n \
  \   Bindbee Embed / Magic Link flow and exchanging the returned temporary_token at\n    GET /api/embedded/v1/connectors/connector_token/{temporary_token}. Rate limits are counted\n    against this token.\n  required_on: >-\n    every operation that reads or writes an end user's data. Organization-level operations\n    (connector list, custom-field configuration, webhook and log reads, integration lookup) take\n    the API key alone.\n  sources:\n  - https://docs.bindbee.dev/api-reference/basics/authentication\n  - https://docs.bindbee.dev/sdk/get-connector-token\nenvironments:\n  selection_mechanism: the API key itself\n  keys:\n  - name: dev_api_key\n    environment: Development\n    note: Cannot access Production. May be shared within a team for testing, per the provider's docs.\n  - name: prod_api_key\n    environment: Production\n    note: Cannot access Development.\n  isolation: >-\n    Complete. Keys, connectors and data never cross between environments, and the environment of a\n\
  \    connector is fixed by whichever key minted its link token.\n  rotation: >-\n    Regenerating a Production key invalidates the previous key immediately; no overlap or grace\n    window is documented.\nscopes:\n  supported: false\n  note: >-\n    There are no OAuth scopes and no permission model in the contract. Authorization is\n    all-or-nothing per key, narrowed only by which connector token accompanies the request. A\n    403 is documented for a connector token used against the wrong API category, or a model whose\n    writes are disabled for that integration — the only granularity Bindbee expresses.\nfailure_modes:\n- status: 401\n  meaning: Missing or invalid bearer credentials.\n  header: WWW-Authenticate challenge returned.\n- status: 403\n  meaning: >-\n    Valid credentials, wrong resource — most often a connector token used on a different API\n    category, or a write attempted on a model where writes are disabled.\ncredential_storage_guidance:\n  source: https://docs.bindbee.dev/api-reference/basics/authentication\n\
  \  note: >-\n    Bindbee advises storing the API key securely after creation because it cannot be retrieved\n    again — only regenerated.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bindbee/refs/heads/main/authentication/bindbee-authentication.yml
summary_line: http/apiKey · 2 schemes
tags:
- ATS
- HR Integration
- HRIS
- Workforce
- Unified API
- Payroll
- LMS
- Employee Data
- Integrations
---
