---
api_key_in: []
api_specs:
- filename: western-power-outage-openapi.yml
  format: yaml
  label: Western Power Outage Web API
  slug: western-power-outage-web-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/western-power/refs/heads/main/openapi/western-power-outage-openapi.yml
- filename: western-power-corporate-web-openapi.yml
  format: yaml
  label: Western Power Corporate Web API
  slug: western-power-corporate-web-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/western-power/refs/heads/main/openapi/western-power-corporate-web-openapi.yml
- filename: western-power-arcgis-outage-openapi.yml
  format: yaml
  label: Western Power Outage Areas Feature Service
  slug: western-power-outage-areas-feature-service
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/western-power/refs/heads/main/openapi/western-power-arcgis-outage-openapi.yml
auth_types:
- none
- esri-token
- session-cookie
description: ''
kind: authentication
layout: security
method: searched
name: Western Power Authentication
name_suffix: Authentication
oauth_flows: []
overview: Western Power secures its APIs with none, esri-token, and session-cookie across 5 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Western Power
provider_slug: western-power
scheme_count: 5
schemes:
- applies_to:
  - openapi/western-power-outage-openapi.yml
  - openapi/western-power-corporate-web-openapi.yml
  - openapi/western-power-arcgis-outage-openapi.yml
  description: Anonymous, unauthenticated HTTPS GET. Verified 200 on 2026-07-27 against /api/corp/outage/all-outages, /api/corp/outage/details/{outageId}, /api/corp/outage/status/{suburb}, /api/search, /api/corp/newsarticles, /api/corp/vacancies and the ArcGIS FeatureServer metadata and query endpoints. No key, token, referer check or origin restriction was required.
  evidence: examples/western-power-all-outages-sample.json
  name: none
  type: none
- applies_to: Western Power Public Secure Services (SLIP)
  description: Esri token authentication after registering a SLIP account on the WA Government platform and agreeing to Western Power's Data Licence Terms and Conditions. Anonymous calls to the MapServer root and to layer 10 both returned HTTP 401 on 2026-07-27.
  name: esri-token
  registration: https://catalogue.data.wa.gov.au/dataset/wp-licence-terms-and-conditions
  token_endpoint: https://token.slip.wa.gov.au
  type: token
- applies_to: data-downloads.slip.wa.gov.au bulk downloads
  description: Form login; an anonymous request for a dataset download returned HTTP 302 to /Account/Login.
  name: slip-download-session
  type: session-cookie
- applies_to: https://services.westernpower.com.au/online/nbu/do/restricted/Home
  description: Username/password login to the restricted Retailer and Generator portal. A commercial and regulatory relationship is a precondition. No API, no interface control document and no machine credential is published for it.
  name: retailer-generator-portal
  type: session-cookie
- applies_to: customer interval and accumulated metering data
  description: Not an authentication scheme at all — a manual gate. A third party registers a business with Western Power (name, ABN, business type, invoicing), then obtains verifiable written customer consent per meter. Data is delivered by email or a web portal. There is no OAuth consent flow, no scopes, no accreditation register and no machine interface at the end of it.
  docs:
  - https://www.westernpower.com.au/issues-enquiries/requests-preferences/registration-for-access-to-energy-data/
  - https://www.westernpower.com.au/issues-enquiries/requests-preferences/verifiable-consent-for-access-to-energy-data/
  name: consumer-energy-data
  type: out-of-band
slug: western-power-authentication
source_filename: western-power-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-27'\nmethod: searched\nsource: >-\n  live probes 2026-07-27 plus the Western Power and DataWA/SLIP access pages; the\n  derive-authentication.py pass found zero securitySchemes because none of the three\n  captured OpenAPI descriptions declares one — every reachable surface is either\n  fully anonymous or gated outside the API layer.\ndocs: https://www.westernpower.com.au/issues-enquiries/requests-preferences/registration-for-access-to-energy-data/\nsummary:\n  types: [none, esri-token, session-cookie]\n  api_key_in: []\n  oauth2_flows: []\n  openid_connect: false\n  note: >-\n    There is no API key, no bearer token, no OAuth 2.0 and no OpenID Connect\n    anywhere in the Western Power estate. The two machine-readable surfaces that\n    answer at all answer anonymously; everything richer is gated by a human\n    registration or a licence agreement, not by a credential an API client can\n    obtain programmatically.\nschemes:\n- name: none\n  type: none\n\
  \  applies_to:\n  - openapi/western-power-outage-openapi.yml\n  - openapi/western-power-corporate-web-openapi.yml\n  - openapi/western-power-arcgis-outage-openapi.yml\n  description: >-\n    Anonymous, unauthenticated HTTPS GET. Verified 200 on 2026-07-27 against\n    /api/corp/outage/all-outages, /api/corp/outage/details/{outageId},\n    /api/corp/outage/status/{suburb}, /api/search, /api/corp/newsarticles,\n    /api/corp/vacancies and the ArcGIS FeatureServer metadata and query endpoints.\n    No key, token, referer check or origin restriction was required.\n  evidence: examples/western-power-all-outages-sample.json\n- name: esri-token\n  type: token\n  applies_to: Western Power Public Secure Services (SLIP)\n  token_endpoint: https://token.slip.wa.gov.au\n  description: >-\n    Esri token authentication after registering a SLIP account on the WA Government\n    platform and agreeing to Western Power's Data Licence Terms and Conditions.\n    Anonymous calls to the MapServer root and\
  \ to layer 10 both returned HTTP 401 on\n    2026-07-27.\n  registration: https://catalogue.data.wa.gov.au/dataset/wp-licence-terms-and-conditions\n- name: slip-download-session\n  type: session-cookie\n  applies_to: data-downloads.slip.wa.gov.au bulk downloads\n  description: >-\n    Form login; an anonymous request for a dataset download returned HTTP 302 to\n    /Account/Login.\n- name: retailer-generator-portal\n  type: session-cookie\n  applies_to: https://services.westernpower.com.au/online/nbu/do/restricted/Home\n  description: >-\n    Username/password login to the restricted Retailer and Generator portal. A\n    commercial and regulatory relationship is a precondition. No API, no interface\n    control document and no machine credential is published for it.\n- name: consumer-energy-data\n  type: out-of-band\n  applies_to: customer interval and accumulated metering data\n  description: >-\n    Not an authentication scheme at all — a manual gate. A third party registers a\n    business\
  \ with Western Power (name, ABN, business type, invoicing), then obtains\n    verifiable written customer consent per meter. Data is delivered by email or a\n    web portal. There is no OAuth consent flow, no scopes, no accreditation register\n    and no machine interface at the end of it.\n  docs:\n  - https://www.westernpower.com.au/issues-enquiries/requests-preferences/registration-for-access-to-energy-data/\n  - https://www.westernpower.com.au/issues-enquiries/requests-preferences/verifiable-consent-for-access-to-energy-data/\ndiscovery:\n  openid_configuration: 404 on www.westernpower.com.au and my.westernpower.com.au (2026-07-27)\n  oauth_authorization_server: 404 on www.westernpower.com.au (2026-07-27)\n  oauth_protected_resource: 404 on www.westernpower.com.au (2026-07-27)\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/western-power/refs/heads/main/authentication/western-power-authentication.yml
summary_line: none/esri-token/session-cookie · 5 schemes
tags:
- Energy
- Australia
- Utilities
- Electricity
- Grid
- Network Distribution
- Smart Metering
- Open Data
- GIS
- Outages
---
