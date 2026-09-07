---
anonymous_access: false
api_key_in: []
api_specs:
- filename: entergy-wordpress-rest-openapi.yml
  format: yaml
  label: Entergy WordPress REST API
  slug: entergy-wordpress-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/entergy/refs/heads/main/openapi/entergy-wordpress-rest-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 4
method: probed
name: Entergy Authentication
name_suffix: Authentication
oauth_flows: []
overview: Entergy declares 4 security scheme(s) across its OpenAPI definitions.
provider_name: Entergy
provider_slug: entergy
scheme_count: 4
schemes:
- anonymous_read: true
  api: entergy-wordpress-rest
  description: The route index at https://www.entergy.com/wp-json/ advertises authentication.application-passwords.endpoints.authorization = https://www.entergy.com/wp-admin/authorize-application.php. This is WordPress core behaviour, available only to accounts that already exist in Entergy's CMS - there is no public registration. Anonymous callers get the public read routes; everything else returns the rest_forbidden envelope with HTTP 401.
  evidence: https://www.entergy.com/wp-json/
  evidence_status: 200
  id: wordpress-application-password
  name: WordPress Application Passwords
  public_registration: false
  scheme: basic
  type: http
- api: entergy-wordpress-rest
  description: Observed in the live Access-Control-Allow-Headers on a wp-json response (Authorization, X-WP-Nonce, Content-Disposition, Content-MD5, Content-Type). This is the first-party browser path used by entergy.com's own front end, not an integration path.
  evidence: https://www.entergy.com/wp-json/wp/v2/posts?per_page=1
  evidence_status: 200
  id: wordpress-cookie-nonce
  in: header
  key_name: X-WP-Nonce
  name: WordPress cookie authentication with nonce
  type: apiKey
- anonymous_read: false
  api: entergy-arcgis
  description: 'https://gis.entergy.com/arcgis/rest/info?f=json reports authInfo.isTokenBasedSecurity = true, tokenServicesUrl = https://gis.entergy.com/arcgis/tokens/ and shortLivedTokenValidity = 60 minutes. The SOAP catalog confirms it independently: RequiresTokens returns Result 1. The service directory itself (/arcgis/rest/services) answers HTTP 200 with {"error":{"code":499,"message":"Token Required"}} - the API is real and reachable, the data is not public. Tokens are issued to Entergy accounts; there is no public request path.'
  evidence: https://gis.entergy.com/arcgis/rest/info?f=json
  evidence_status: 200
  id: arcgis-token
  in: query
  key_name: token
  name: ArcGIS Server short-lived token
  public_registration: false
  type: apiKey
- api: entergy-green-button
  description: Entergy Texas operates Green Button Connect My Data, which by the NAESB REQ.21 ESPI standard is an OAuth 2.0 authorization-code flow between a registered third-party service provider and the utility Data Custodian. Entergy publishes the PROGRAM (https://myentergyadvisor.entergy.com/greenbutton/welcome, HTTP 200) and a vendor registration form (/greenbutton/green-vendor, HTTP 200) but publishes NO endpoint URLs, NO scope list and NO client-registration document anonymously. The flow is asserted here only as the standard's mandated shape; no Entergy-specific authorization, token or resource URL is recorded, because none was served.
  evidence: https://myentergyadvisor.entergy.com/greenbutton/green-vendor
  evidence_status: 200
  gated_behind: vendor registration form
  id: green-button-espi
  name: NAESB REQ.21 ESPI (Green Button Connect My Data) authorization
  public_registration: false
  type: oauth2
slug: entergy-authentication
source_filename: entergy-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-06'\nmethod: probed\nsource: >-\n  https://www.entergy.com/wp-json/ (route index, HTTP 200) plus\n  https://gis.entergy.com/arcgis/rest/info?f=json (HTTP 200) and a live SOAP RequiresTokens\n  call against https://gis.entergy.com/arcgis/services (HTTP 200, Result 1).\nname: Entergy authentication profile\nsummary: >-\n  Entergy runs no developer identity platform. The two machine-readable surfaces it serves\n  each carry their own vendor-native auth model, and neither issues developer credentials\n  through a self-service portal.\nschemes:\n  - id: wordpress-application-password\n    api: entergy-wordpress-rest\n    type: http\n    scheme: basic\n    name: WordPress Application Passwords\n    description: >-\n      The route index at https://www.entergy.com/wp-json/ advertises\n      authentication.application-passwords.endpoints.authorization =\n      https://www.entergy.com/wp-admin/authorize-application.php. This is WordPress core\n      behaviour, available\
  \ only to accounts that already exist in Entergy's CMS - there is no\n      public registration. Anonymous callers get the public read routes; everything else\n      returns the rest_forbidden envelope with HTTP 401.\n    public_registration: false\n    anonymous_read: true\n    evidence: https://www.entergy.com/wp-json/\n    evidence_status: 200\n  - id: wordpress-cookie-nonce\n    api: entergy-wordpress-rest\n    type: apiKey\n    in: header\n    key_name: X-WP-Nonce\n    name: WordPress cookie authentication with nonce\n    description: >-\n      Observed in the live Access-Control-Allow-Headers on a wp-json response\n      (Authorization, X-WP-Nonce, Content-Disposition, Content-MD5, Content-Type). This is the\n      first-party browser path used by entergy.com's own front end, not an integration path.\n    evidence: https://www.entergy.com/wp-json/wp/v2/posts?per_page=1\n    evidence_status: 200\n  - id: arcgis-token\n    api: entergy-arcgis\n    type: apiKey\n    in: query\n    key_name:\
  \ token\n    name: ArcGIS Server short-lived token\n    description: >-\n      https://gis.entergy.com/arcgis/rest/info?f=json reports\n      authInfo.isTokenBasedSecurity = true, tokenServicesUrl =\n      https://gis.entergy.com/arcgis/tokens/ and shortLivedTokenValidity = 60 minutes. The\n      SOAP catalog confirms it independently: RequiresTokens returns Result 1. The service\n      directory itself (/arcgis/rest/services) answers HTTP 200 with\n      {\"error\":{\"code\":499,\"message\":\"Token Required\"}} - the API is real and reachable, the\n      data is not public. Tokens are issued to Entergy accounts; there is no public request path.\n    public_registration: false\n    anonymous_read: false\n    evidence: https://gis.entergy.com/arcgis/rest/info?f=json\n    evidence_status: 200\n  - id: green-button-espi\n    api: entergy-green-button\n    type: oauth2\n    name: NAESB REQ.21 ESPI (Green Button Connect My Data) authorization\n    description: >-\n      Entergy Texas operates\
  \ Green Button Connect My Data, which by the NAESB REQ.21 ESPI\n      standard is an OAuth 2.0 authorization-code flow between a registered third-party\n      service provider and the utility Data Custodian. Entergy publishes the PROGRAM\n      (https://myentergyadvisor.entergy.com/greenbutton/welcome, HTTP 200) and a vendor\n      registration form (/greenbutton/green-vendor, HTTP 200) but publishes NO endpoint URLs,\n      NO scope list and NO client-registration document anonymously. The flow is asserted here\n      only as the standard's mandated shape; no Entergy-specific authorization, token or\n      resource URL is recorded, because none was served.\n    public_registration: false\n    gated_behind: vendor registration form\n    evidence: https://myentergyadvisor.entergy.com/greenbutton/green-vendor\n    evidence_status: 200\nnot_found:\n  - No /.well-known/openid-configuration on any Entergy host (all 404).\n  - No /.well-known/oauth-authorization-server on any Entergy host (all\
  \ 404).\n  - No developer portal, no API key issuance page, no client-credentials documentation.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/entergy/refs/heads/main/authentication/entergy-authentication.yml
summary_line: 4 schemes
tags:
- Electricity
- Energy
- Fortune 500
- Utility
- Nuclear
- Power Generation
- Louisiana
- Geospatial
---
