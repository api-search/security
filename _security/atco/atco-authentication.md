---
api_key_in: []
api_specs:
- filename: atco-query-api-openapi.yml
  format: yaml
  label: ATCO Query API
  slug: atco-query-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/atco/refs/heads/main/openapi/atco-query-api-openapi.yml
- filename: atco-service-api-openapi.yml
  format: yaml
  label: ATCO Service API
  slug: atco-service-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/atco/refs/heads/main/openapi/atco-service-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
method: searched
name: Atco Authentication
name_suffix: Authentication
oauth_flows: []
overview: ATCO declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: ATCO
provider_slug: atco
scheme_count: 0
schemes: []
slug: atco-authentication
source_filename: atco-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-27'\nmethod: searched\nsource: >-\n  Live anonymous probes of the ATCO Electric hosting capacity feature service and of every\n  ATCO web property, 2026-07-27. Confirms the negative finding already recorded in review.yml.\ndocs: null\ndocs_note: >-\n  ATCO publishes no API authentication documentation of any kind. There is no developer portal,\n  no /docs, no /api and no auth page on atco.com, electric.atco.com, gas.atco.com or\n  atcoenergy.com. This profile was established by probing the running service rather than by\n  reading a document.\nsummary:\n  types: []\n  api_key_in: []\n  oauth2_flows: []\n  anonymous: true\nschemes: []\nprofile:\n  scheme: none\n  detail: >-\n    The only public ATCO API — the ATCO Electric DER hosting capacity feature service — accepts\n    completely anonymous HTTPS requests. No `token` query parameter is required, no\n    Authorization header is honoured or needed, and no ArcGIS token error (code 498/499) is\n    returned\
  \ for an unauthenticated request. A GET against\n    /FeatureServer/0/query?where=1=1&returnCountOnly=true&f=json returned {\"count\":880623} with\n    no credential of any kind on 2026-07-27.\n  signup_required: false\n  api_key_required: false\n  oauth2: false\n  openid_connect: false\n  mutual_tls: false\n  referer_check: false\n  licence_click_through: false\n  cors:\n    access_control_allow_origin: '*'\n    note: >-\n      The service returns a wildcard CORS header, so it is directly callable from browser\n      JavaScript with no proxy.\nupstream_token_service:\n  note: >-\n    The ArcGIS platform underneath does support token-based security — /arcgis/rest/info reports\n    isTokenBasedSecurity true with tokenServicesUrl https://www.arcgis.com/sharing/generateToken.\n    That is the Esri ArcGIS Online platform capability, not something ATCO has enabled on this\n    service. The AGO_HostingCapacity service item is shared publicly (access \"public\"), so no\n    token is used.\n \
  \ rest_info: https://services7.arcgis.com/cw2emabghNLkoYlB/arcgis/rest/info?f=json\n  token_services_url: https://www.arcgis.com/sharing/generateToken\nconsumer_data_auth:\n  available: false\n  note: >-\n    There is no machine authentication path to a customer's own energy usage or billing data.\n    ATCO Energy routes My Account (https://myaccount.atcoenergy.com, HTTP 301) to\n    https://store.atco.com/ccrz__CCSiteLogin, a Salesforce CloudCraze human commerce login. No\n    OAuth authorization server, no consent flow, no third-party onboarding and no client\n    registration exists. /.well-known/openid-configuration returns 404 on every ATCO host.\ndiscovery_probes:\n- url: https://www.atco.com/.well-known/openid-configuration\n  status: 404\n- url: https://www.atcoenergy.com/.well-known/openid-configuration\n  status: 404\n- url: https://electric.atco.com/.well-known/openid-configuration\n  status: 404\n- url: https://gas.atco.com/.well-known/openid-configuration\n  status: 404\n\
  - url: https://services7.arcgis.com/.well-known/oauth-authorization-server\n  status: 403\nrelated:\n- scopes/: not applicable — no OAuth surface exists, so no scope artifact is emitted\n- conventions/atco-conventions.yml\n- security/atco-domain-security.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/atco/refs/heads/main/authentication/atco-authentication.yml
summary_line: 0 schemes
tags:
- Energy
- Canada
- Utilities
- Electricity
- Gas
- Grid
- Distribution
- Transmission
- DER
- Solar
- Renewables
- Open Data
- Geospatial
- Alberta
---
