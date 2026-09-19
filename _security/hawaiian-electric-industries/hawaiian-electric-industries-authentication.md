---
anonymous_access: true
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: probed
name: Hawaiian Electric Industries Authentication
name_suffix: Authentication
oauth_flows: []
overview: Hawaiian Electric Industries declares 4 security scheme(s) across its OpenAPI definitions.
provider_name: Hawaiian Electric Industries
provider_slug: hawaiian-electric-industries
scheme_count: 4
schemes:
- base_url: https://services5.arcgis.com/gfBpz2hbsVDgru6D/ArcGIS/rest/services
  detail: 'Anonymous GET succeeds. No API key, token, referer check or CORS restriction was encountered. The response carries `vary: X-Esri-Authorization`, so an ArcGIS token is accepted if presented but is not required for read access.'
  evidence: https://services5.arcgis.com/gfBpz2hbsVDgru6D/ArcGIS/rest/services/extLVM/FeatureServer/0/query?where=1%3D1&returnCountOnly=true&f=json
  http_status: 200
  id: anonymous
  required: false
  surface: ArcGIS REST feature services (public)
  type: none
- base_url: https://outagemap-api-heco.azurewebsites.net/api/v1
  detail: 'Answers `HTTP/1.1 401 Unauthorized` with `WWW-Authenticate: Bearer` and an empty body. Tokens are minted for the map''s own Blazor client by a companion service at https://ext-access-heco.azurewebsites.net/ (v1), named in the app''s public appsettings.json with an AccessTokenLifetime of 120. No token endpoint, registration flow, scope list or OAuth metadata document is published — there is no way for a third party to obtain a credential. Treat this as a private backend, not an available API.'
  evidence: https://outagemap-api-heco.azurewebsites.net/api/v1/outages
  http_status: 401
  id: bearer-internal
  required: true
  scheme: bearer
  surface: Outage map backend (first-party, undocumented)
  type: http
- base_url: https://eservice.hawaiianelectric.com/bdisu/logon.sap
  detail: SAP Business Server Page logon for retail customers. Human web session only; no programmatic or delegated-access path is offered, and Green Button data is reached through it as a file download rather than through an ESPI API.
  evidence: https://www.hawaiianelectric.com/clean-energy-hawaii/grid-modernization-technologies/advanced-meters/my-energy-use-portal
  id: customer-login-sap
  required: true
  surface: Customer self-service portal (My Energy Use, Green Button download)
  type: session
- base_url: https://forms.hawaiianelectric.com/login
  detail: Account-based web login used by customers and solar contractors to file interconnection and service applications. Human web application; no API.
  evidence: https://www.hawaiianelectric.com/products-and-services/smart-renewable-energy-programs/cit-cid
  id: contractor-login-cit
  required: true
  surface: Customer Interconnection Tool (CIT)
  type: session
slug: hawaiian-electric-industries-authentication
source_filename: hawaiian-electric-industries-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-13'\nmethod: probed\nsource: >-\n  Live probes of https://services5.arcgis.com/gfBpz2hbsVDgru6D/ArcGIS/rest/services,\n  https://outagemap-api-heco.azurewebsites.net/api/v1/outages and the login surfaces linked from\n  www.hawaiianelectric.com.\ndocs: null\nnote: >-\n  Hawaiian Electric publishes NO authentication documentation. Everything below was established by\n  probe, not by reading a provider auth page, and is recorded as observed behaviour.\nschemes:\n  - id: anonymous\n    type: none\n    surface: ArcGIS REST feature services (public)\n    base_url: https://services5.arcgis.com/gfBpz2hbsVDgru6D/ArcGIS/rest/services\n    required: false\n    evidence: https://services5.arcgis.com/gfBpz2hbsVDgru6D/ArcGIS/rest/services/extLVM/FeatureServer/0/query?where=1%3D1&returnCountOnly=true&f=json\n    http_status: 200\n    detail: >-\n      Anonymous GET succeeds. No API key, token, referer check or CORS restriction was\n      encountered. The response carries\
  \ `vary: X-Esri-Authorization`, so an ArcGIS token is\n      accepted if presented but is not required for read access.\n  - id: bearer-internal\n    type: http\n    scheme: bearer\n    surface: Outage map backend (first-party, undocumented)\n    base_url: https://outagemap-api-heco.azurewebsites.net/api/v1\n    required: true\n    evidence: https://outagemap-api-heco.azurewebsites.net/api/v1/outages\n    http_status: 401\n    detail: >-\n      Answers `HTTP/1.1 401 Unauthorized` with `WWW-Authenticate: Bearer` and an empty body.\n      Tokens are minted for the map's own Blazor client by a companion service at\n      https://ext-access-heco.azurewebsites.net/ (v1), named in the app's public appsettings.json\n      with an AccessTokenLifetime of 120. No token endpoint, registration flow, scope list or\n      OAuth metadata document is published — there is no way for a third party to obtain a\n      credential. Treat this as a private backend, not an available API.\n  - id: customer-login-sap\n\
  \    type: session\n    surface: Customer self-service portal (My Energy Use, Green Button download)\n    base_url: https://eservice.hawaiianelectric.com/bdisu/logon.sap\n    required: true\n    evidence: https://www.hawaiianelectric.com/clean-energy-hawaii/grid-modernization-technologies/advanced-meters/my-energy-use-portal\n    detail: >-\n      SAP Business Server Page logon for retail customers. Human web session only; no\n      programmatic or delegated-access path is offered, and Green Button data is reached through\n      it as a file download rather than through an ESPI API.\n  - id: contractor-login-cit\n    type: session\n    surface: Customer Interconnection Tool (CIT)\n    base_url: https://forms.hawaiianelectric.com/login\n    required: true\n    evidence: https://www.hawaiianelectric.com/products-and-services/smart-renewable-energy-programs/cit-cid\n    detail: >-\n      Account-based web login used by customers and solar contractors to file interconnection and\n      service\
  \ applications. Human web application; no API.\ndiscovery_documents:\n  openid_configuration: null\n  oauth_authorization_server: null\n  oauth_protected_resource: null\n  note: >-\n    None served. www.hei.com answers HTTP 200 with an 11-byte \"Invalid key\" body for every\n    /.well-known/ path — a catch-all, not metadata. See\n    well-known/hawaiian-electric-industries-well-known.yml.\ndelegated_identity:\n  supported: false\n  note: >-\n    No OAuth consent flow exists for customer energy data. Green Button Connect My Data, which\n    would be the standard delegated path in this sector, is not published.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hawaiian-electric-industries/refs/heads/main/authentication/hawaiian-electric-industries-authentication.yml
summary_line: 4 schemes
tags:
- Energy
- Utilities
- Electricity
- Grid
- Holding Company
- Hawaii
- Fortune 1000
- Geospatial
- ArcGIS
- Open Data
- Locational Value Map
- EV Charging
---
