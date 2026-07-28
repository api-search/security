---
api_key_in:
- query
api_specs:
- filename: eia-api-v2-openapi.yml
  format: yaml
  label: EIA Open Data API (APIv2)
  slug: eia-open-data-api-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eia/refs/heads/main/openapi/eia-api-v2-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Eia Authentication
name_suffix: Authentication
oauth_flows: []
overview: EIA secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: EIA
provider_slug: eia
scheme_count: 1
schemes:
- applied: globally, via the root-level security requirement in the spec
  in: query
  name: api_key
  parameter: api_key
  sources:
  - openapi/eia-api-v2-openapi.yml
  type: apiKey
slug: eia-authentication
source_filename: eia-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-27'\nmethod: searched\nsource: openapi/eia-api-v2-openapi.yml\ndocs: https://www.eia.gov/opendata/documentation.php\nregistration: https://www.eia.gov/opendata/register.php\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - query\n  oauth2_flows: []\n  free: true\n  self_serve: true\n  approval_required: false\nschemes:\n- name: api_key\n  type: apiKey\n  in: query\n  parameter: api_key\n  applied: globally, via the root-level security requirement in the spec\n  sources:\n  - openapi/eia-api-v2-openapi.yml\nmodel: |\n  A single free API key, passed as the api_key query parameter on every APIv2 request. EIA\n  states explicitly that the key must appear in the URL and will NOT be detected in HTTP\n  headers, even though other query parameters MAY be sent in the request body\n  (application/x-www-form-urlencoded on GET, or a JSON DataParams body on the POST form of a\n  /data route) to work around URL length limits. There is no OAuth, no OIDC, no bearer token,\n\
  \  no mutual TLS, no scopes and no per-resource authorization - every key sees the same public\n  statistical data.\nissuance:\n  form: https://www.eia.gov/opendata/register.php\n  fields:\n  - First Name (required)\n  - Last Name (required)\n  - Email (required)\n  - Category that best describes you/your organization (required)\n  - Reason to use this API\n  - Agreement to the API Terms of Service (required)\n  - Optional opt-in for email notification of API changes\n  delivery: Emailed automatically to the address supplied; no human review, no accreditation,\n    no licence to sign.\n  sender: developer@eia.gov - EIA asks that this address be whitelisted in spam filters.\n  recovery: '\"Forgot API Key\" flow linked from https://www.eia.gov/opendata/'\n  cost: free\nunauthenticated_surface:\n  bulk_download: https://api.eia.gov/bulk/manifest.txt and every /bulk/*.zip dataset are\n    retrievable with NO key at all.\n  spec_download: https://www.eia.gov/opendata/eia-api-swagger.zip is\
  \ anonymous.\n  console: https://www.eia.gov/opendata/browser/ is anonymous.\nenforcement:\n  missing_key: HTTP 403 with {\"error\":{\"code\":\"API_KEY_MISSING\",\"message\":\"No api_key was\n    supplied.  Please register for one at https://www.eia.gov/opendata/register.php\"}} -\n    verified live 2026-07-27.\n  invalid_key: HTTP 403 with {\"error\":{\"code\":\"API_KEY_INVALID\", ...}} - verified live\n    2026-07-27 with a 40-character bogus key.\n  throttled_key: The key is automatically and temporarily suspended above the published\n    thresholds and automatically reactivated. See rate-limits/eia-rate-limits.yml.\n  embeds: The chart-widget embed now also requires a key; unkeyed embeds render\n    API_KEY_MISSING.\ntransport:\n  https_only: true\n  note: APIv2 is HTTPS-only. APIv1 also served plain http; EIA flagged that http would \"end\n    soon\" as part of the v2 migration.\nkey_handling_risk: Because the key travels in the query string it is exposed in browser\n  history, referrer\
  \ headers, proxy logs and server access logs, and the documented embed\n  pattern places a live key in public page HTML. There is no key rotation UI - recovery is via\n  the Forgot API Key flow.\nterms_of_service: https://www.eia.gov/opendata/register.php\nscopes: none\nscopes_note: No OAuth scopes exist; scopes/ is deliberately absent for this provider.\nrelated:\n  conventions: conventions/eia-conventions.yml\n  errors: errors/eia-problem-types.yml\n  rate_limits: rate-limits/eia-rate-limits.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/eia/refs/heads/main/authentication/eia-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Energy
- United States
- Energy Markets
- Electricity
- Natural Gas
- Petroleum
- Coal
- Nuclear
- Renewables
- Grid
- Emissions
- Government
- Open Data
- Energy Statistics
---
