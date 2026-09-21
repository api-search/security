---
anonymous_access: false
api_key_in: []
api_specs:
- filename: bidmachine-io-placement-management-openapi.yml
  format: yaml
  label: BidMachine Placement Management API
  slug: bidmachine-placement-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bidmachine-io/refs/heads/main/openapi/bidmachine-io-placement-management-openapi.yml
- filename: bidmachine-io-reporting-openapi.yml
  format: yaml
  label: BidMachine Reporting API
  slug: bidmachine-reporting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bidmachine-io/refs/heads/main/openapi/bidmachine-io-reporting-openapi.yml
auth_types:
- http
description: 'BidMachine''s REST APIs use HTTP authentication only — no API keys, no OAuth 2.0, no OIDC. The credentials are the publisher''s dashboard login and password. The Reporting API takes them as HTTP Basic on every request (a 401 answers WWW-Authenticate: Basic realm="Reporting API"). The Placement Management API exchanges the same Basic credentials at POST /auth for a short-lived bearer token ({token, expires}) and requires Authorization: Bearer <token> on every placement call; when a call returns 401 the token has expired and the client re-authenticates. All placement operations are scoped to sources the authenticated publisher owns (403 otherwise). No token revocation endpoint, no scopes and no service accounts are documented. The OpenRTB auction surface authenticates by source id in the endpoint path (https://api-eu.bidmachine.io/auction/prebid/${source_id}) issued per partner, not by a header.'
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Bidmachine Io Authentication
name_suffix: Authentication
oauth_flows: []
overview: BidMachine secures its APIs with http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: BidMachine
provider_slug: bidmachine-io
scheme_count: 2
schemes:
- docs: https://developers.bidmachine.io/api/bidmachine-reporting-api
  name: basicAuth
  scheme: basic
  sources:
  - openapi/bidmachine-io-placement-management-openapi.yml
  - openapi/bidmachine-io-reporting-openapi.yml
  type: http
  used_by:
  - openapi/bidmachine-io-placement-management-openapi.yml#getAccessToken
  - openapi/bidmachine-io-reporting-openapi.yml#retrieveSspReportData
  - openapi/bidmachine-io-reporting-openapi.yml#retrieveBidderReportData
  - openapi/bidmachine-io-reporting-openapi.yml#retrieveP2pRevenueReportData
- docs: https://developers.bidmachine.io/api/get-access-token
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/bidmachine-io-placement-management-openapi.yml
  token_endpoint: POST https://api-eu.bidmachine.io/api/v1/auth (Basic credentials in; {token, expires} out)
  type: http
  used_by:
  - openapi/bidmachine-io-placement-management-openapi.yml#listPlacements
  - openapi/bidmachine-io-placement-management-openapi.yml#createPlacement
  - openapi/bidmachine-io-placement-management-openapi.yml#updatePlacement
  - openapi/bidmachine-io-placement-management-openapi.yml#deletePlacement
slug: bidmachine-io-authentication
source_filename: bidmachine-io-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: searched\nsource: openapi/bidmachine-io-placement-management-openapi.yml, openapi/bidmachine-io-reporting-openapi.yml\ndocs: https://developers.bidmachine.io/api/get-access-token\ndescription: >-\n  BidMachine's REST APIs use HTTP authentication only — no API keys, no OAuth 2.0, no OIDC. The\n  credentials are the publisher's dashboard login and password. The Reporting API takes them as HTTP\n  Basic on every request (a 401 answers WWW-Authenticate: Basic realm=\"Reporting API\"). The Placement\n  Management API exchanges the same Basic credentials at POST /auth for a short-lived bearer token\n  ({token, expires}) and requires Authorization: Bearer <token> on every placement call; when a call\n  returns 401 the token has expired and the client re-authenticates. All placement operations are\n  scoped to sources the authenticated publisher owns (403 otherwise). No token revocation endpoint,\n  no scopes and no service accounts are documented.\
  \ The OpenRTB auction surface authenticates by\n  source id in the endpoint path (https://api-eu.bidmachine.io/auction/prebid/${source_id}) issued\n  per partner, not by a header.\nsummary:\n  types:\n    - http\n  http_schemes:\n    - basic\n    - bearer\n  api_key_in: []\n  oauth2_flows: []\n  credential: dashboard login and password (https://dashboard.bidmachine.io/sign-in)\n  token_lifetime: short-lived; `expires` (date-time) is returned with the token, the exact TTL is not published\n  observed:\n    - {url: 'https://api-eu.bidmachine.io/api/v1/report/ssp?start=2026-09-01&end=2026-09-02', status: 401, www_authenticate: 'Basic realm=\"Reporting API\"'}\n    - {url: 'https://api-eu.bidmachine.io/api/v1/publisher/sources/1/placements', status: 401, body: 'HTML \"Authentication required\"'}\nschemes:\n  - name: basicAuth\n    type: http\n    scheme: basic\n    docs: https://developers.bidmachine.io/api/bidmachine-reporting-api\n    used_by:\n      - openapi/bidmachine-io-placement-management-openapi.yml#getAccessToken\n\
  \      - openapi/bidmachine-io-reporting-openapi.yml#retrieveSspReportData\n      - openapi/bidmachine-io-reporting-openapi.yml#retrieveBidderReportData\n      - openapi/bidmachine-io-reporting-openapi.yml#retrieveP2pRevenueReportData\n    sources:\n      - openapi/bidmachine-io-placement-management-openapi.yml\n      - openapi/bidmachine-io-reporting-openapi.yml\n  - name: bearerAuth\n    type: http\n    scheme: bearer\n    docs: https://developers.bidmachine.io/api/get-access-token\n    token_endpoint: POST https://api-eu.bidmachine.io/api/v1/auth (Basic credentials in; {token, expires} out)\n    used_by:\n      - openapi/bidmachine-io-placement-management-openapi.yml#listPlacements\n      - openapi/bidmachine-io-placement-management-openapi.yml#createPlacement\n      - openapi/bidmachine-io-placement-management-openapi.yml#updatePlacement\n      - openapi/bidmachine-io-placement-management-openapi.yml#deletePlacement\n    sources:\n      - openapi/bidmachine-io-placement-management-openapi.yml\n\
  related:\n  conventions: conventions/bidmachine-io-conventions.yml\n  errors: errors/bidmachine-io-problem-types.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bidmachine-io/refs/heads/main/authentication/bidmachine-io-authentication.yml
summary_line: http · 2 schemes
tags:
- Advertising
- AdTech
- Mobile Advertising
- Ad Exchange
- Ad Mediation
- In-App Bidding
- OpenRTB
- App Monetization
- Programmatic Advertising
- Mobile SDK
- Reporting
- Company
---
