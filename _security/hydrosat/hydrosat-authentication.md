---
api_key_in: []
api_specs:
- filename: hydrosat-stac-openapi.json
  format: json
  label: Hydrosat Discovery STAC API
  slug: hydrosat-discovery-stac-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hydrosat/refs/heads/main/openapi/hydrosat-stac-openapi.json
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Hydrosat Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Hydrosat secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Hydrosat
provider_slug: hydrosat
scheme_count: 1
schemes:
- credential_model: client_id + client_secret (per API client)
  flow: clientCredentials
  grant: client_credentials
  name: OAuth2ClientCredentials
  request_content_type: application/x-www-form-urlencoded
  sources:
  - https://satdocs.hydrosat.com/stac-api-reference-and-specification/authentication
  token_ttl_seconds: 3600
  token_type: Bearer
  token_url: https://auth.hydrosat.com/oauth2/token
  type: oauth2
slug: hydrosat-authentication
source_filename: hydrosat-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://satdocs.hydrosat.com/stac-api-reference-and-specification/authentication.md\ndocs: https://satdocs.hydrosat.com/stac-api-reference-and-specification/authentication\nsummary:\n  types: [oauth2]\n  oauth2_flows: [clientCredentials]\n  api_key_in: []\n  note: >-\n    The published STAC OpenAPI (openapi/hydrosat-stac-openapi.json) declares no\n    securitySchemes, but the Discovery STAC API is bearer-token protected. The\n    auth model below is captured from the provider's authentication docs.\nschemes:\n  - name: OAuth2ClientCredentials\n    type: oauth2\n    flow: clientCredentials\n    token_url: https://auth.hydrosat.com/oauth2/token\n    token_type: Bearer\n    token_ttl_seconds: 3600\n    credential_model: client_id + client_secret (per API client)\n    grant: client_credentials\n    request_content_type: application/x-www-form-urlencoded\n    sources: [https://satdocs.hydrosat.com/stac-api-reference-and-specification/authentication]\n\
  client_provisioning:\n  portal: https://discover.hydrosat.com/\n  where: Account > API Clients (Org Admin role required)\n  max_clients_per_account: 4\n  secret_shown_once: true\n  docs: https://satdocs.hydrosat.com/discovery-portal/managing-api-clients\nusage: >-\n  Exchange client_id/client_secret at the token URL for a short-lived (3600s)\n  bearer access_token, then send Authorization: Bearer <token> to every\n  https://stac.hydrosat.com/ request; refresh before expiry.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hydrosat/refs/heads/main/authentication/hydrosat-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Company
- Satellite Imagery
- Thermal Infrared
- Geospatial
- Earth Observation
- Remote Sensing
- STAC
- Agriculture
- Water Management
- Data
---
