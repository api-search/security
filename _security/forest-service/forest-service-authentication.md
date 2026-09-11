---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 0
method: probed
name: Forest Service Authentication
name_suffix: Authentication
oauth_flows: []
overview: Forest Service declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: Forest Service
provider_slug: forest-service
scheme_count: 0
schemes: []
slug: forest-service-authentication
source_filename: forest-service-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-10'\nmethod: probed\nsource: >-\n  Anonymous live calls to all four Forest Service API surfaces plus /.well-known/ discovery\n  probes, 2026-09-10.\nnote: >-\n  All four public Forest Service API surfaces are fully anonymous. No key, token, account,\n  registration or referrer restriction stands between a caller and a 200 — every response\n  recorded in this repository was obtained with a bare curl and no credential of any kind. This\n  is the single most agent-relevant fact about the estate: there is nothing to onboard to and\n  nothing to rotate. It is also why scopes/ is deliberately absent — there is no OAuth surface to\n  derive scopes from.\nsummary:\n  schemes_declared: 0\n  auth_required: false\n  registration_required: false\n  model: open public data, unauthenticated\nsecurity_schemes: []\nsurfaces:\n  - api: Forest Service Research Data Archive Web Service\n    base_url: https://www.fs.usda.gov/rds/archive/webservice\n    auth: none\n    verified:\n\
  \      - url: https://www.fs.usda.gov/rds/archive/webservice/efrs\n        status: 200\n        detail: 200 text/xml, 32 experimental forests returned, no credential sent.\n      - url: https://www.fs.usda.gov/rds/archive/webservice/organizations\n        status: 200\n        detail: 200 text/xml, 405 organizations returned.\n      - url: https://www.fs.usda.gov/rds/archive/webservice/oaipmh?verb=Identify\n        status: 200\n    session_note: >-\n      The service sets a PHPSESSID cookie and an F5 BIGipServer cookie on response. Neither is\n      required on the request — the calls above were made cookieless.\n  - api: FIADB-API / EVALIDator\n    base_url: https://apps.fs.usda.gov/fiadb-api\n    auth: none\n    verified:\n      - url: https://apps.fs.usda.gov/fiadb-api/fullreport?rselected=Land%20Use%20-%20Major&cselected=Land%20use&snum=79&wc=102020&outputFormat=NJSON\n        status: 200\n        detail: >-\n          200 application/json, 34 KB of population estimates with standard\
  \ errors, no credential\n          sent. Response carries Access-Control-Allow-Origin \"*\", so the API is callable directly\n          from a browser origin.\n    session_note: >-\n      Sets an evalidator.session cookie (Secure, HttpOnly) on response; not required on request.\n  - api: FSGeodata EDW map services (ArcGIS REST)\n    base_url: https://apps.fs.usda.gov/arcx/rest/services\n    auth: none\n    verified:\n      - url: https://apps.fs.usda.gov/arcx/rest/services?f=json\n        status: 200\n      - url: https://apps.fs.usda.gov/arcx/rest/services/EDW?f=json\n        status: 200\n        detail: 144 MapServer services enumerated anonymously.\n    note: >-\n      ArcGIS Server supports token authentication, but no /arcx/tokens/generateToken challenge is\n      raised for these services — they are published to the anonymous role.\n  - api: FSGeodata RDW map services (ArcGIS REST, fsgisx01)\n    base_url: https://apps.fs.usda.gov/fsgisx01/rest/services\n    auth: none\n    verified:\n\
  \      - url: https://apps.fs.usda.gov/fsgisx01/rest/services?f=json\n        status: 200\n  - api: U.S. Forest Service Geospatial Data Discovery (DCAT-US catalog)\n    base_url: https://data-usfs.hub.arcgis.com\n    auth: none\n    verified:\n      - url: https://data-usfs.hub.arcgis.com/api/feed/dcat-us/1.1.json\n        status: 200\n        detail: 200 application/json, ~2 MB catalog returned anonymously.\ndiscovery_probes:\n  - url: https://www.fs.usda.gov/.well-known/openid-configuration\n    status: 404\n  - url: https://www.fs.usda.gov/.well-known/oauth-authorization-server\n    status: 404\n  - url: https://apps.fs.usda.gov/.well-known/oauth-authorization-server\n    status: 500\ntransport:\n  https_required: true\n  hsts: true\n  detail: >-\n    Every host redirects to HTTPS and returns Strict-Transport-Security max-age=31536000;\n    www.fs.usda.gov adds includeSubDomains and preload. See\n    security/forest-service-domain-security.yml.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/forest-service/refs/heads/main/authentication/forest-service-authentication.yml
summary_line: 0 schemes
tags:
- Agriculture
- Federal-Government
- Forests
- Geospatial
- Open-Data
- Research-Data
- Forest-Inventory
- Wildfire
- Public-Lands
- Environment
---
