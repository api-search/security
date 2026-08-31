---
api_key_in: []
api_specs:
- filename: ontario-energy-board-applications-before-the-oeb-api-openapi.yml
  format: yaml
  label: Ontario Energy Board Applications before the OEB API
  slug: ontario-energy-board-applications-before-the-oeb-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ontario-energy-board/refs/heads/main/openapi/ontario-energy-board-applications-before-the-oeb-api-openapi.yml
- filename: ontario-energy-board-current-electricity-rates-general-service-50-kw-rate-class-api-openapi.yml
  format: yaml
  label: Ontario Energy Board Current Electricity Rates (General Service < 50 kW Rate Class) API
  slug: ontario-energy-board-current-electricity-rates-general-service-50-kw-rate-class-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ontario-energy-board/refs/heads/main/openapi/ontario-energy-board-current-electricity-rates-general-service-50-kw-rate-class-api-openapi.yml
- filename: ontario-energy-board-current-electricity-rates-residential-rate-class-api-openapi.yml
  format: yaml
  label: Ontario Energy Board Current Electricity Rates (Residential Rate Class) API
  slug: ontario-energy-board-current-electricity-rates-residential-rate-class-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ontario-energy-board/refs/heads/main/openapi/ontario-energy-board-current-electricity-rates-residential-rate-class-api-openapi.yml
- filename: ontario-energy-board-current-natural-gas-rates-residential-rate-classes-api-openapi.yml
  format: yaml
  label: Ontario Energy Board Current Natural Gas Rates (Residential Rate Classes) API
  slug: ontario-energy-board-current-natural-gas-rates-residential-rate-classes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ontario-energy-board/refs/heads/main/openapi/ontario-energy-board-current-natural-gas-rates-residential-rate-classes-api-openapi.yml
- filename: ontario-energy-board-electricity-and-natural-gas-distributors-service-areas-api-openapi.yml
  format: yaml
  label: Ontario Energy Board Electricity and Natural Gas Distributors - Service Areas API
  slug: ontario-energy-board-electricity-and-natural-gas-distributors-service-areas-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ontario-energy-board/refs/heads/main/openapi/ontario-energy-board-electricity-and-natural-gas-distributors-service-areas-api-openapi.yml
- filename: ontario-energy-board-electricity-distributor-complaints-received-by-the-oeb-api-openapi.yml
  format: yaml
  label: Ontario Energy Board Electricity Distributor Complaints Received by the OEB API
  slug: ontario-energy-board-electricity-distributor-complaints-received-by-the-oeb-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ontario-energy-board/refs/heads/main/openapi/ontario-energy-board-electricity-distributor-complaints-received-by-the-oeb-api-openapi.yml
- filename: ontario-energy-board-electricity-distributor-performance-scorecard-api-openapi.yml
  format: yaml
  label: Ontario Energy Board Electricity Distributor Performance – Scorecard API
  slug: ontario-energy-board-electricity-distributor-performance-scorecard-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ontario-energy-board/refs/heads/main/openapi/ontario-energy-board-electricity-distributor-performance-scorecard-api-openapi.yml
- filename: ontario-energy-board-electricity-reporting-record-keeping-requirements-rrr-section-api-openapi.yml
  format: yaml
  label: 'Ontario Energy Board Electricity Reporting & Record Keeping Requirements (RRR): Section ... API'
  slug: ontario-energy-board-electricity-reporting-record-keeping-requirements-rrr-section-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ontario-energy-board/refs/heads/main/openapi/ontario-energy-board-electricity-reporting-record-keeping-requirements-rrr-section-api-openapi.yml
- filename: ontario-energy-board-historical-regulated-price-plan-electricity-rates-api-openapi.yml
  format: yaml
  label: Ontario Energy Board Historical Regulated Price Plan Electricity Rates API
  slug: ontario-energy-board-historical-regulated-price-plan-electricity-rates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ontario-energy-board/refs/heads/main/openapi/ontario-energy-board-historical-regulated-price-plan-electricity-rates-api-openapi.yml
- filename: ontario-energy-board-licensed-market-participants-api-openapi.yml
  format: yaml
  label: Ontario Energy Board Licensed Market Participants API
  slug: ontario-energy-board-licensed-market-participants-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ontario-energy-board/refs/heads/main/openapi/ontario-energy-board-licensed-market-participants-api-openapi.yml
- filename: ontario-energy-board-records-api-openapi.yml
  format: yaml
  label: Ontario Energy Board Records API
  slug: ontario-energy-board-records-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ontario-energy-board/refs/heads/main/openapi/ontario-energy-board-records-api-openapi.yml
- filename: ontario-energy-board-search-metadata-api-openapi.yml
  format: yaml
  label: Ontario Energy Board Search Metadata API
  slug: ontario-energy-board-search-metadata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ontario-energy-board/refs/heads/main/openapi/ontario-energy-board-search-metadata-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
method: derived
name: Ontario Energy Board Authentication
name_suffix: Authentication
oauth_flows: []
overview: Ontario Energy Board declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: Ontario Energy Board
provider_slug: ontario-energy-board
scheme_count: 0
schemes: []
slug: ontario-energy-board-authentication
source_filename: ontario-energy-board-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-27'\nmethod: derived\nsource: >-\n  Live anonymous probes of https://www.oeb.ca and https://www.rds.oeb.ca on 2026-07-27, plus\n  openapi/ontario-energy-board-open-data-openapi.yml and openapi/ontario-energy-board-rds-openapi.yml\nnote: >-\n  The Ontario Energy Board operates no authentication of any kind on either of its public data\n  surfaces. There is no developer portal, no API key, no OAuth client registration, no signup and no\n  terms click-through. Every one of the 38 operations described in this repo's two OpenAPI documents\n  was executed anonymously — no Authorization header, no cookie, no token — and returned the real\n  payload. This is recorded as a positive, verified finding, not as an absence: for a regulator\n  publishing rate, performance and case-record data under an open licence, unauthenticated is the\n  correct posture, and it is the opposite of what the utilities the OEB supervises do with the\n  consumer data they hold.\nmodel: anonymous\n\
  authentication_required: false\nschemes: []\nsurfaces:\n- api: OEB Open Data\n  host: https://www.oeb.ca\n  authentication: none\n  evidence: >-\n    33 dataset files fetched anonymously with HTTP 200 on 2026-07-27 (see x-evidence on every\n    operation in openapi/ontario-energy-board-open-data-openapi.yml). No 401 or 403 was returned by\n    any of them.\n- api: OEB Regulatory Document Search (RDS)\n  host: https://www.rds.oeb.ca/CMWebDrawer\n  authentication: none\n  evidence: >-\n    Record search (HTTP 200 JSON), document download (HTTP 200 application/pdf, 339,517 bytes) and\n    the search-clause vocabulary (HTTP 200 text/javascript) all served anonymously.\n  caveat: >-\n    The server does set ServiceStack session cookies (ss-pid, ss-id, Secure/HttpOnly/SameSite=Lax) on\n    every response. They are not required — requests made without carrying cookies forward succeed —\n    but they mean the underlying Content Manager instance does maintain an anonymous session.\n  partial_authorization_note:\
  \ >-\n    One surface behaves as if it were access-controlled: GET /Record/{uri} returns HTTP 500 with\n    \"Error retrieving data for property RecordContainer. Access denied.\" (TrimErrorCode 22760), while\n    the document bytes under the same URI are served without complaint. This is an internal Content\n    Manager ACL leaking through the anonymous WebDrawer projection, not an authentication challenge —\n    no WWW-Authenticate header is returned and no credential would change the result for a public\n    caller.\nnot_applicable:\n- api_keys\n- oauth2\n- openid_connect\n- mutual_tls\n- jwt\n- hmac_request_signing\n- basic_auth\nmandate_context: >-\n  The OEB holds no customer meter, usage or billing data, so it operates no Green Button Connect My\n  Data authorization server and issues no OAuth credentials. The consented, OAuth-2.0-protected\n  energy-data surfaces in Ontario belong to the rate-regulated utilities the OEB supervises under\n  O. Reg. 633/21 - see all/hydro-one/ and\
  \ all/toronto-hydro/ for that side of the mandate.\ntransport:\n  https_required: true\n  tls_version_observed: TLSv1.3\n  hsts: true\n  hsts_max_age: 31536000\n  detail: security/ontario-energy-board-domain-security.yml\nrelated:\n- security/ontario-energy-board-domain-security.yml\n- conventions/ontario-energy-board-conventions.yml\n- conformance/ontario-energy-board-conformance.yml\n- openapi/ontario-energy-board-rds-openapi.yml\n- openapi/ontario-energy-board-open-data-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ontario-energy-board/refs/heads/main/authentication/ontario-energy-board-authentication.yml
summary_line: 0 schemes
tags:
- Energy
- Canada
- Ontario
- Utilities
- Electricity
- Gas
- Green Button
- Smart Metering
- Energy Markets
- Regulator
- Open Data
- Grid
---
