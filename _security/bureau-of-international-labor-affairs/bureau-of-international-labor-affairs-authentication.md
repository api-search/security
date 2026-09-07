---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Bureau Of International Labor Affairs Authentication
name_suffix: Authentication
oauth_flows: []
overview: Bureau of International Labor Affairs declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Bureau of International Labor Affairs
provider_slug: bureau-of-international-labor-affairs
scheme_count: 1
schemes:
- also_accepted_in: header
  applies_to:
  - /v4/get/{agency}/{endpoint}/{format}
  - /v4/get/{agency}/{endpoint}/{format}/metadata
  description: '"X-API-KEY (string, required): User''s API key for authentication." Documented on the portal''s Getting Started page. The portal''s own examples pass it as a query string parameter, e.g. https://apiprod.dol.gov/v4/get/{agency}/{endpoint}/json/metadata?X-API-KEY={api_key}'
  id: dol-open-data-api-key
  in: query
  key_format: '"Your API key will look like a mixture of numbers, letters, and special characters." No prefix is documented.'
  key_management: https://dataportal.dol.gov/api-keys
  keys_per_account: 5
  name: X-API-KEY
  obtain: Register an account at https://dataportal.dol.gov/registration, complete the API User Questionnaire, and accept the Terms of Service. A key is issued to the account after a short propagation delay.
  required: true
  rotation_policy: Not published. Additional keys (up to 5) can be created for different purposes, client applications or automation, which is the documented substitute for rotation.
  type: apiKey
slug: bureau-of-international-labor-affairs-authentication
source_filename: bureau-of-international-labor-affairs-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-05'\nmethod: searched\nsource: >-\n  https://dataportal.dol.gov/getting-started and https://dataportal.dol.gov/api-keys\n  — the DOL Open Data Portal is a React single-page app, so the published reference\n  text was read out of its shipped bundle\n  (https://dataportal.dol.gov/static/js/main.1788ccf8.js), which is the same content\n  the portal renders to a human.\nprovider: Bureau of International Labor Affairs\nproviderId: bureau-of-international-labor-affairs\nsummary: >-\n  ILAB does not run its own API gateway. Its seven public datasets are served through\n  the department-wide U.S. Department of Labor Open Data Portal API at\n  https://apiprod.dol.gov/v4, which authenticates with a single long-lived API key\n  passed as X-API-KEY. There is no OAuth, no OIDC, no scopes and no token exchange.\nbase_url: https://apiprod.dol.gov/v4\nschemes:\n  - id: dol-open-data-api-key\n    type: apiKey\n    name: X-API-KEY\n    in: query\n    also_accepted_in: header\n\
  \    required: true\n    applies_to:\n      - /v4/get/{agency}/{endpoint}/{format}\n      - /v4/get/{agency}/{endpoint}/{format}/metadata\n    description: >-\n      \"X-API-KEY (string, required): User's API key for authentication.\" Documented on\n      the portal's Getting Started page. The portal's own examples pass it as a query\n      string parameter, e.g.\n      https://apiprod.dol.gov/v4/get/{agency}/{endpoint}/json/metadata?X-API-KEY={api_key}\n    key_format: >-\n      \"Your API key will look like a mixture of numbers, letters, and special characters.\"\n      No prefix is documented.\n    obtain: >-\n      Register an account at https://dataportal.dol.gov/registration, complete the API\n      User Questionnaire, and accept the Terms of Service. A key is issued to the account\n      after a short propagation delay.\n    key_management: https://dataportal.dol.gov/api-keys\n    keys_per_account: 5\n    rotation_policy: >-\n      Not published. Additional keys (up to 5) can be\
  \ created for different purposes,\n      client applications or automation, which is the documented substitute for rotation.\nunauthenticated_surface:\n  - path: /v4/datasets\n    url: https://apiprod.dol.gov/v4/datasets\n    status: 200\n    note: >-\n      The dataset catalogue endpoint answers anonymously and is paginated\n      (meta.current_page / next_page / total_pages / total_count). Verified 2026-09-05:\n      42 datasets across 5 pages, 7 of them ILAB (agency.abbr \"ILAB\", agency_id 24).\n      This is the only DOL v4 route observed to serve data without a key.\nobserved_failures:\n  - status: 401\n    where: /v4/get/ilab/{endpoint}/json/metadata with no key\n    body: >-\n      The API key is either incorrect or missing from your query. If you are using the\n      API Query Builder in the Open Data Portal, please Sign in and try again, otherwise\n      please correct your key.\n    note: Plain-text body, not JSON, and not RFC 9457.\nnot_present:\n  oauth2: false\n  openIdConnect:\
  \ false\n  mutualTLS: false\n  http_bearer: false\n  scopes: >-\n    None. The key is unscoped — it grants read access to the whole public catalogue.\n    No scopes/ artifact is written for this provider (see the pipeline's OAuth-only rule).\nmaintainers:\n  - FN: Kin Lane\n    email: kin@apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bureau-of-international-labor-affairs/refs/heads/main/authentication/bureau-of-international-labor-affairs-authentication.yml
summary_line: 1 scheme
tags:
- Federal-Government
- International
- Labor
- Standards
- Child Labor
- Forced Labor
- Human Trafficking
---
