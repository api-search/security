---
api_key_in:
- query
- header
api_specs:
- filename: hydro-quebec-catalog-api-openapi.yml
  format: yaml
  label: Hydro-Québec Catalog API
  slug: hydro-quebec-catalog-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hydro-quebec/refs/heads/main/openapi/hydro-quebec-catalog-api-openapi.yml
- filename: hydro-quebec-dataset-api-openapi.yml
  format: yaml
  label: Hydro-Québec Dataset API
  slug: hydro-quebec-dataset-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hydro-quebec/refs/heads/main/openapi/hydro-quebec-dataset-api-openapi.yml
auth_types:
- none
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Hydro Quebec Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Hydro-Québec secures its APIs with none, apiKey, and oauth2 across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Hydro-Québec
provider_slug: hydro-quebec
scheme_count: 3
schemes:
- declared: true
  description: API key to make authenticated requests.
  in: query
  name: apikey
  parameter: apikey
  preference_note: Platform docs recommend the header form over the query parameter because headers are not stored in browser history or server logs, minimizing exposure risk.
  preferred: false
  sources:
  - openapi/hydro-quebec-open-data-explore-api-v2-0-openapi.json
  - openapi/hydro-quebec-open-data-explore-api-v2-1-openapi.json
  type: apiKey
- declared: false
  description: The same API key supplied in the Authorization header. Documented by the platform as good practice and the recommended form.
  format: Apikey <API_KEY>
  in: header
  name: apikeyHeader
  parameter: Authorization
  preferred: true
  sources:
  - https://help.opendatasoft.com/apis/ods-explore-v2/explore_v2.1.html
  type: apiKey
- declared: false
  description: Platform OAuth2 authorization code flow for third-party applications acting on behalf of a user, compliant with RFC 6749 and using Bearer tokens per RFC 6750.
  detail: scopes/hydro-quebec-scopes.yml
  flows:
  - authorizationUrl: https://donnees.hydroquebec.com/oauth2/authorize/
    flow: authorizationCode
    scope_count: 1
    scopes:
    - all
    tokenUrl: https://donnees.hydroquebec.com/oauth2/token/
    verified: '2026-07-27'
  name: oauth2
  sources:
  - https://help.opendatasoft.com/apis/ods-explore-v2/explore_v2.1.html
  type: oauth2
slug: hydro-quebec-authentication
source_filename: hydro-quebec-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-27'\nmethod: searched\nsource: >-\n  openapi/hydro-quebec-open-data-explore-api-v2-0-openapi.json,\n  openapi/hydro-quebec-open-data-explore-api-v2-1-openapi.json,\n  https://help.opendatasoft.com/apis/ods-explore-v2/explore_v2.1.html,\n  and live probes of donnees.hydroquebec.com on 2026-07-27\ndocs: https://help.opendatasoft.com/apis/ods-explore-v2/explore_v2.1.html\nnote: >-\n  Upgraded from the mechanically derived profile. The harvested specs declare only a single apiKey\n  scheme in the query string; the platform documentation and live probes show two further schemes\n  the spec omits — the same API key in an Authorization header, and a full OAuth2 authorization\n  code flow. The governing fact for consumers is that none of it is required: Hydro-Québec's\n  catalog is public and anonymous.\nsummary:\n  required: false\n  anonymous_access: true\n  types: [none, apiKey, oauth2]\n  api_key_in: [query, header]\n  oauth2_flows: [authorizationCode]\n  declared_in_spec:\
  \ [apiKey/query]\n  undeclared_in_spec: [apiKey/header, oauth2]\nanonymous:\n  supported: true\n  verified: '2026-07-27'\n  evidence: >-\n    GET https://donnees.hydroquebec.com/api/explore/v2.1/catalog/datasets?limit=1 returned HTTP 200\n    with total_count 26 and no credentials of any kind.\n  scope_of_access: All 26 public datasets, every one of the 16 operations, both v2.0 and v2.1.\nschemes:\n- name: apikey\n  type: apiKey\n  in: query\n  parameter: apikey\n  description: API key to make authenticated requests.\n  declared: true\n  preferred: false\n  preference_note: >-\n    Platform docs recommend the header form over the query parameter because headers are not\n    stored in browser history or server logs, minimizing exposure risk.\n  sources:\n  - openapi/hydro-quebec-open-data-explore-api-v2-0-openapi.json\n  - openapi/hydro-quebec-open-data-explore-api-v2-1-openapi.json\n- name: apikeyHeader\n  type: apiKey\n  in: header\n  parameter: Authorization\n  format: 'Apikey <API_KEY>'\n\
  \  description: >-\n    The same API key supplied in the Authorization header. Documented by the platform as good\n    practice and the recommended form.\n  declared: false\n  preferred: true\n  sources: [https://help.opendatasoft.com/apis/ods-explore-v2/explore_v2.1.html]\n- name: oauth2\n  type: oauth2\n  description: >-\n    Platform OAuth2 authorization code flow for third-party applications acting on behalf of a\n    user, compliant with RFC 6749 and using Bearer tokens per RFC 6750.\n  declared: false\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://donnees.hydroquebec.com/oauth2/authorize/\n    tokenUrl: https://donnees.hydroquebec.com/oauth2/token/\n    scopes: [all]\n    scope_count: 1\n    verified: '2026-07-27'\n  sources: [https://help.opendatasoft.com/apis/ods-explore-v2/explore_v2.1.html]\n  detail: scopes/hydro-quebec-scopes.yml\nkey_management:\n  self_service: true\n  console: https://donnees.hydroquebec.com/account/\n  create_revoke: true\n  identity_model:\
  \ >-\n    A key authenticates as the user who created it and carries that user's rights, so keys are\n    personal and must not be shared. Finer-grained key permissions require the platform's API key\n    Automation API.\nunauthenticated_behaviour:\n  status_on_private_catalog: 401\n  status_on_hydro_quebec: 200\n  note: >-\n    The 401 Unauthorized declared on all 16 operations applies to private Opendatasoft portals.\n    The Hydro-Québec portal is public, so anonymous requests succeed and 401 is not reachable in\n    normal use.\ndiscovery:\n  openid_configuration: 404\n  oauth_authorization_server: 404\n  note: >-\n    Neither RFC 8414 nor OIDC discovery metadata is published, so the OAuth2 endpoints above must\n    be configured from documentation rather than discovered.\nconsumer_data:\n  customer_api: false\n  note: >-\n    There is no authentication path to an individual customer's own electricity consumption. No\n    customer-facing API, no Green Button Download My Data or Connect\
  \ My Data, and no third-party\n    consent flow exist. A customer's usage is reachable only by logging into the Espace client web\n    portal as themselves.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hydro-quebec/refs/heads/main/authentication/hydro-quebec-authentication.yml
summary_line: none/apiKey/oauth2 · 3 schemes
tags:
- Energy
- Canada
- Utilities
- Electricity
- Grid
- Energy Markets
- Renewables
- Open Data
- Demand Response
- Carbon
---
