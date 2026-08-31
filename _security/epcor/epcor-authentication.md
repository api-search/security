---
api_key_in: []
api_specs:
- filename: epcor-boundaries-api-openapi.yml
  format: yaml
  label: EPCOR Boundaries API
  slug: epcor-boundaries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/epcor/refs/heads/main/openapi/epcor-boundaries-api-openapi.yml
- filename: epcor-catalog-api-openapi.yml
  format: yaml
  label: EPCOR Catalog API
  slug: epcor-catalog-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/epcor/refs/heads/main/openapi/epcor-catalog-api-openapi.yml
- filename: epcor-infrastructure-api-openapi.yml
  format: yaml
  label: EPCOR Infrastructure API
  slug: epcor-infrastructure-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/epcor/refs/heads/main/openapi/epcor-infrastructure-api-openapi.yml
- filename: epcor-power-outages-api-openapi.yml
  format: yaml
  label: EPCOR Power Outages API
  slug: epcor-power-outages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/epcor/refs/heads/main/openapi/epcor-power-outages-api-openapi.yml
- filename: epcor-service-areas-api-openapi.yml
  format: yaml
  label: EPCOR Service Areas API
  slug: epcor-service-areas-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/epcor/refs/heads/main/openapi/epcor-service-areas-api-openapi.yml
- filename: epcor-us-water-outages-api-openapi.yml
  format: yaml
  label: EPCOR Us Water Outages API
  slug: epcor-us-water-outages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/epcor/refs/heads/main/openapi/epcor-us-water-outages-api-openapi.yml
- filename: epcor-water-outages-api-openapi.yml
  format: yaml
  label: EPCOR Water Outages API
  slug: epcor-water-outages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/epcor/refs/heads/main/openapi/epcor-water-outages-api-openapi.yml
auth_types:
- none
- delegated-consent
description: ''
kind: authentication
layout: security
method: probed
name: Epcor Authentication
name_suffix: Authentication
oauth_flows: []
overview: EPCOR secures its APIs with none and delegated-consent across 4 declared security schemes, as derived from its OpenAPI definitions.
provider_name: EPCOR
provider_slug: epcor
scheme_count: 4
schemes:
- detail: 'All 36 production feature services in the epcor_outages ArcGIS Online folder are shared publicly. Every probed metadata document and query returned 200 with no credential, no Referer restriction and no key parameter. `security: []` in the derived OpenAPI reflects this.'
  name: anonymous
  sources:
  - openapi/epcor-outages-arcgis-openapi.yml
  surface: EPCOR public ArcGIS feature services
  type: none
  verified: '2026-07-27'
- detail: Several services advertise Create/Update/Delete/Editing/Extract/ChangeTracking capabilities. Writing to an ArcGIS Online hosted feature service requires an ArcGIS token (Esri platform authentication, not an EPCOR credential). This is inferred from the advertised capabilities and the ArcGIS platform contract - no write was attempted and no token endpoint of EPCOR's own exists.
  in: query
  name: arcgis-token
  parameter_name: token
  sources:
  - openapi/epcor-outages-arcgis-openapi.yml
  surface: EPCOR public ArcGIS feature services (write side)
  type: apiKey
  verified: false
- detail: Every path on the Green Button portal host 302s into /Connect/Authorize and serves an EPCOR-skinned single page login application. Only the account holder, authenticated, can download their own XML.
  name: customer-login
  sources:
  - https://epcorgas.savagedata.com/
  surface: EPCOR Ontario Green Button - Download My Data
  type: interactive-login
  verified: '2026-07-27'
- detail: EPCOR describes customer-authorized ongoing sharing of energy usage, billing and account data with registered third-party vendors "using security tokens", revocable from a Data Shares tab. This is the Green Button Connect My Data pattern, which the NAESB ESPI standard implements over OAuth 2.0 - but EPCOR never names OAuth, never publishes an authorization or token endpoint, and never publishes scopes. A vendor must first be approved through the registration application.
  name: green-button-cmd-consent
  sources:
  - https://www.epcor.com/ca/en/on/collingwood-area/account/manage-account/green-button.html
  - https://epcorgasonboarding.savagedata.com/
  surface: EPCOR Ontario Green Button - Connect My Data
  type: delegated-consent
  verification_note: /.well-known/openid-configuration, /.well-known/oauth-authorization-server and /.well-known/oauth-protected-resource were requested anonymously on both savagedata hosts on 2026-07-27. All returned HTTP 200 with the site's HTML single page app rather than a discovery document - a soft 404. No authorization server metadata, no scopes and no token endpoint are publicly discoverable.
  verified: false
slug: epcor-authentication
source_filename: epcor-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-27'\nmethod: probed\nsource: >-\n  live probes of https://services6.arcgis.com/Ji2rusuWXDFSqNsP/ArcGIS/rest/services,\n  https://epcorgas.savagedata.com/ and https://epcorgasonboarding.savagedata.com/, plus EPCOR's own Green\n  Button pages\nsummary:\n  types: [none, delegated-consent]\n  api_key_in: []\n  oauth2_flows: []\n  note: >-\n    EPCOR has two utterly different access models and no published authentication documentation for either.\n    The public geospatial surface needs no credential at all; the regulated consumer-data surface needs a\n    customer login and, for third parties, an application-approval process with no public technical contract.\nschemes:\n  - name: anonymous\n    surface: EPCOR public ArcGIS feature services\n    type: none\n    sources: [openapi/epcor-outages-arcgis-openapi.yml]\n    detail: >-\n      All 36 production feature services in the epcor_outages ArcGIS Online folder are shared publicly. Every\n      probed metadata\
  \ document and query returned 200 with no credential, no Referer restriction and no key\n      parameter. `security: []` in the derived OpenAPI reflects this.\n    verified: '2026-07-27'\n  - name: arcgis-token\n    surface: EPCOR public ArcGIS feature services (write side)\n    type: apiKey\n    in: query\n    parameter_name: token\n    sources: [openapi/epcor-outages-arcgis-openapi.yml]\n    detail: >-\n      Several services advertise Create/Update/Delete/Editing/Extract/ChangeTracking capabilities. Writing to\n      an ArcGIS Online hosted feature service requires an ArcGIS token (Esri platform authentication, not an\n      EPCOR credential). This is inferred from the advertised capabilities and the ArcGIS platform contract -\n      no write was attempted and no token endpoint of EPCOR's own exists.\n    verified: false\n  - name: customer-login\n    surface: EPCOR Ontario Green Button - Download My Data\n    type: interactive-login\n    sources: [https://epcorgas.savagedata.com/]\n\
  \    detail: >-\n      Every path on the Green Button portal host 302s into /Connect/Authorize and serves an EPCOR-skinned\n      single page login application. Only the account holder, authenticated, can download their own XML.\n    verified: '2026-07-27'\n  - name: green-button-cmd-consent\n    surface: EPCOR Ontario Green Button - Connect My Data\n    type: delegated-consent\n    sources:\n      - https://www.epcor.com/ca/en/on/collingwood-area/account/manage-account/green-button.html\n      - https://epcorgasonboarding.savagedata.com/\n    detail: >-\n      EPCOR describes customer-authorized ongoing sharing of energy usage, billing and account data with\n      registered third-party vendors \"using security tokens\", revocable from a Data Shares tab. This is the\n      Green Button Connect My Data pattern, which the NAESB ESPI standard implements over OAuth 2.0 - but\n      EPCOR never names OAuth, never publishes an authorization or token endpoint, and never publishes scopes.\n \
  \     A vendor must first be approved through the registration application.\n    verified: false\n    verification_note: >-\n      /.well-known/openid-configuration, /.well-known/oauth-authorization-server and\n      /.well-known/oauth-protected-resource were requested anonymously on both savagedata hosts on 2026-07-27.\n      All returned HTTP 200 with the site's HTML single page app rather than a discovery document - a soft 404.\n      No authorization server metadata, no scopes and no token endpoint are publicly discoverable.\nscopes:\n  published: false\n  detail: No OAuth scope surface is discoverable, so no scopes/ artifact is emitted for this provider.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/epcor/refs/heads/main/authentication/epcor-authentication.yml
summary_line: none/delegated-consent · 4 schemes
tags:
- Energy
- Canada
- Utilities
- Electricity
- Natural Gas
- Water
- Green Button
- Smart Metering
- Grid
- Ontario
- Alberta
- Outages
- Geospatial
- Open Data
---
