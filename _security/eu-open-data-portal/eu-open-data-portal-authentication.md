---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: eu-open-data-portal-hub-search-openapi.yaml
  format: yaml
  label: EU Open Data Portal Search API (hub-search)
  slug: eu-open-data-portal-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eu-open-data-portal/refs/heads/main/openapi/eu-open-data-portal-hub-search-openapi.yaml
- filename: eu-open-data-portal-hub-repo-openapi.yaml
  format: yaml
  label: EU Open Data Portal Registry API (hub-repo)
  slug: eu-open-data-portal-registry-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eu-open-data-portal/refs/heads/main/openapi/eu-open-data-portal-hub-repo-openapi.yaml
- filename: eu-open-data-portal-mqa-metrics-cache-openapi.yaml
  format: yaml
  label: EU Open Data Portal MQA Metrics Cache API
  slug: eu-open-data-portal-mqa-metrics-cache-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eu-open-data-portal/refs/heads/main/openapi/eu-open-data-portal-mqa-metrics-cache-openapi.yaml
- filename: eu-open-data-portal-mqa-shacl-openapi.yaml
  format: yaml
  label: EU Open Data Portal SHACL Validation API
  slug: eu-open-data-portal-mqa-shacl-validation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eu-open-data-portal/refs/heads/main/openapi/eu-open-data-portal-mqa-shacl-openapi.yaml
- filename: eu-open-data-portal-mqa-reporter-openapi.yaml
  format: yaml
  label: EU Open Data Portal MQA Metrics Reporter API
  slug: eu-open-data-portal-mqa-metrics-reporter-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eu-open-data-portal/refs/heads/main/openapi/eu-open-data-portal-mqa-reporter-openapi.yaml
- filename: eu-open-data-portal-hub-statistics-swagger.json
  format: json
  label: EU Open Data Portal Statistics API
  slug: eu-open-data-portal-statistics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eu-open-data-portal/refs/heads/main/openapi/eu-open-data-portal-hub-statistics-swagger.json
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Eu Open Data Portal Authentication
name_suffix: Authentication
oauth_flows: []
overview: EU Open Data Portal secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: EU Open Data Portal
provider_slug: eu-open-data-portal
scheme_count: 2
schemes:
- in: header
  name: ApiKeyAuth
  parameter: X-API-Key
  sources:
  - openapi/eu-open-data-portal-hub-repo-openapi.yaml
  - openapi/eu-open-data-portal-hub-search-openapi.yaml
  - openapi/eu-open-data-portal-mqa-metrics-cache-openapi.yaml
  type: apiKey
- bearerFormat: JWT
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/eu-open-data-portal-hub-repo-openapi.yaml
  - openapi/eu-open-data-portal-hub-search-openapi.yaml
  - openapi/eu-open-data-portal-mqa-metrics-cache-openapi.yaml
  type: http
slug: eu-open-data-portal-authentication
source_filename: eu-open-data-portal-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-07'\nmethod: searched\nsource: openapi/ securitySchemes across hub-repo, hub-search and the MQA metrics cache, upgraded from https://dataeuropa.gitlab.io/data-provider-manual/api-documentation/api-access-control/\n  and https://dataeuropa.gitlab.io/data-provider-manual/api-documentation/api-store/\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\n  public_read: true\n  note: 'Reads are anonymous across every API — search, MQA metrics, MQA reporter, SHACL validation, statistics and SPARQL\n    all answer without a credential (verified live). Credentials are only needed to WRITE into a catalogue, and they\n    are not self-service: access is granted by the portal team to a catalogue you are responsible for.'\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  sources:\n  - openapi/eu-open-data-portal-hub-repo-openapi.yaml\n  - openapi/eu-open-data-portal-hub-search-openapi.yaml\n  - openapi/eu-open-data-portal-mqa-metrics-cache-openapi.yaml\n\
  - name: BearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/eu-open-data-portal-hub-repo-openapi.yaml\n  - openapi/eu-open-data-portal-hub-search-openapi.yaml\n  - openapi/eu-open-data-portal-mqa-metrics-cache-openapi.yaml\ndocs: https://dataeuropa.gitlab.io/data-provider-manual/api-documentation/api-access-control/\nflows:\n- name: Service account (client credentials via the access-control middleware)\n  steps:\n  - POST https://data.europa.eu/auth/middleware/login/service with JSON {client_id, client_secret}\n  - 'Response: {\"access_token\": \"...\"}'\n  - 'Send the token as Authorization: Bearer <token> to hub-repo and hub-store'\n  audience: hub-repo, hub-store\n  source: https://dataeuropa.gitlab.io/data-provider-manual/api-documentation/api-access-control/\n- name: EU Login user + UMA 2.0 party token (Keycloak realm DEU)\n  steps:\n  - POST https://data.europa.eu/auth/realms/DEU/protocol/openid-connect/token with grant_type=password, client_id=piveau-hub-ui,\n\
  \    username, password — returns a user token (expires_in 300, refresh_expires_in 1800, scope 'email profile')\n  - 'POST the same token endpoint with grant_type=urn:ietf:params:oauth:grant-type:uma-ticket and audience=piveau-hub-repo,\n    carrying the user token as Authorization: Bearer — returns the party token'\n  - Use the party token to manage datasets in data.europa.eu\n  audience: piveau-hub-repo\n  token_ttl_seconds: 300\n  refresh_ttl_seconds: 1800\n  source: https://dataeuropa.gitlab.io/data-provider-manual/api-documentation/api-access-control/\n- name: Catalogue-scoped API key\n  steps:\n  - Send the key in the X-API-Key header\n  note: Declared as ApiKeyAuth in all three write-bearing contracts; issuance is handled by the portal team, not documented\n    as self-service.\n  source: openapi/eu-open-data-portal-hub-repo-openapi.yaml\nidentity_provider:\n  type: keycloak\n  realm: DEU\n  token_endpoint: https://data.europa.eu/auth/realms/DEU/protocol/openid-connect/token\n \
  \ middleware_endpoint: https://data.europa.eu/auth/middleware/login/service\n  discovery_document: https://data.europa.eu/auth/realms/DEU/.well-known/openid-configuration\n  discovery_status: 403\n  discovery_note: The realm is real and documented, but its OIDC discovery document is blocked at the edge (HTTP 403\n    probed 2026-09-07), so a client cannot auto-configure.\naccess_control:\n  model: catalogue-scoped, plus ODRL policy-based access control on datasets\n  note: hub-search 5.3.7 added policy-based access control evaluating ODRL constraints on datasets against JWT claims,\n    and 5.3.9 made multiple ODRL policies combine as AND restrictions (service changelog).\n  source: https://gitlab.com/dataeuropa/hub/search/-/blob/master/CHANGELOG.md\ngaps:\n- No scopes are documented anywhere — the observed OIDC scope string is the default \"email profile\", and no scopes/ artifact\n  is emitted because there is no scope surface to record.\n- Unauthorized and Forbidden are declared as\
  \ null entries in hub-search components.responses while 401/403 are referenced\n  by operations.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/eu-open-data-portal/refs/heads/main/authentication/eu-open-data-portal-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Government
- Open Data
- SPARQL
- EU
- Regulatory
- Linked Data
- DCAT-AP
- Data Quality
- Metadata
- Catalogs
---
