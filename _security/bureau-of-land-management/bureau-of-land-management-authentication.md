---
anonymous_access: true
api_key_in: []
api_specs:
- filename: bureau-of-land-management-gbp-hub-search-openapi.json
  format: json
  label: BLM GBP Hub Search API (OGC API - Records)
  slug: blm-gbp-hub-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bureau-of-land-management/refs/heads/main/openapi/bureau-of-land-management-gbp-hub-search-openapi.json
auth_types:
- none
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
mechanism_count: 3
method: probed
name: Bureau Of Land Management Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- implicit
overview: Bureau of Land Management secures its APIs with none, oauth2, and openIdConnect across 6 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and implicit flow(s).
provider_name: Bureau of Land Management
provider_slug: bureau-of-land-management
scheme_count: 6
schemes:
- evidence: The document declares no components.securitySchemes and no security[]. All 17 operations were called anonymously on 2026-09-05 and returned 200. An optional `token` query parameter exists on the item operations for reaching private ArcGIS items; it is not required for BLM's public catalog.
  name: anonymous
  sources:
  - openapi/bureau-of-land-management-gbp-hub-search-openapi.json
  surface: GBP Hub Search API (OGC API - Records)
  type: none
- evidence: Every /rest/info reports authInfo.isTokenBasedSecurity = false. Service directory, layer metadata and /query were all exercised anonymously on 2026-09-05.
  name: anonymous
  sources:
  - openapi/bureau-of-land-management-arcgis-service-inventory.json
  surface: ArcGIS Server REST (13 instances on gis.blm.gov)
  type: none
- evidence: GetCapabilities returned HTTP 200 with no authentication on all seven services fetched.
  name: anonymous
  sources:
  - openapi/bureau-of-land-management-sma-wms-capabilities.xml
  surface: OGC WMS (gis.blm.gov/arcgis/services)
  type: none
- evidence: RFC 8414 metadata, HTTP 200, issuer https://blm-egis.maps.arcgis.com, grant_types_supported [authorization_code, implicit], code_challenge_methods_supported ["S256"]. Needed only to publish or reach non-public items; BLM's published content is open.
  flows:
  - authorizationUrl: https://blm-egis.maps.arcgis.com/sharing/rest/oauth2/authorize
    flow: authorizationCode
    pkce: S256
    tokenUrl: https://blm-egis.maps.arcgis.com/sharing/rest/oauth2/token
  - authorizationUrl: https://blm-egis.maps.arcgis.com/sharing/rest/oauth2/authorize
    flow: implicit
  name: arcgis-online-oauth2
  sources:
  - well-known/bureau-of-land-management-blm-egis-arcgis-oauth-authorization-server.json
  surface: BLM ArcGIS Online organization (blm-egis.maps.arcgis.com)
  type: oauth2
- endpoints:
    authorization: https://mlrs.blm.gov/services/oauth2/authorize
    end_session: https://mlrs.blm.gov/services/auth/idp/oidc/logout
    introspection: https://mlrs.blm.gov/services/oauth2/introspect
    jwks_uri: https://mlrs.blm.gov/id/keys
    registration: https://mlrs.blm.gov/services/oauth2/register
    revocation: https://mlrs.blm.gov/services/oauth2/revoke
    token: https://mlrs.blm.gov/services/oauth2/token
    userinfo: https://mlrs.blm.gov/services/oauth2/userinfo
  evidence: HTTP 200 anonymously on 2026-09-05. Every other probed path on this host answered 401. The 36 advertised scopes are the stock Salesforce platform scope set (api, web, openid, refresh_token, cdp_*, pardot_api, ...), not a BLM-authored permission model — see scopes/bureau-of-land-management-scopes.yml.
  issuer: https://mlrs.blm.gov
  name: mlrs-oidc
  openIdConnectUrl: https://mlrs.blm.gov/.well-known/openid-configuration
  sources:
  - well-known/bureau-of-land-management-mlrs-openid-configuration.json
  surface: Mineral and Land Records System (mlrs.blm.gov)
  type: openIdConnect
- endpoints:
    authorization: https://glorecords.blm.gov/services/oauth2/authorize
    end_session: https://glorecords.blm.gov/services/auth/idp/oidc/logout
    introspection: https://glorecords.blm.gov/services/oauth2/introspect
    jwks_uri: https://glorecords.blm.gov/id/keys
    registration: https://glorecords.blm.gov/services/oauth2/register
    revocation: https://glorecords.blm.gov/services/oauth2/revoke
    token: https://glorecords.blm.gov/services/oauth2/token
    userinfo: https://glorecords.blm.gov/services/oauth2/userinfo
  evidence: HTTP 200 anonymously on 2026-09-05; all other paths on this host answered 401.
  issuer: https://glorecords.blm.gov
  name: glorecords-oidc
  openIdConnectUrl: https://glorecords.blm.gov/.well-known/openid-configuration
  sources:
  - well-known/bureau-of-land-management-glorecords-openid-configuration.json
  surface: General Land Office Records (glorecords.blm.gov)
  type: openIdConnect
slug: bureau-of-land-management-authentication
source_filename: bureau-of-land-management-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-05'\nmethod: probed\nsource: >-\n  openapi/bureau-of-land-management-gbp-hub-search-openapi.json (no securitySchemes declared),\n  live probes of gis.blm.gov/<instance>/rest/info, and the OIDC/OAuth discovery documents saved\n  verbatim in well-known/, all 2026-09-05.\ndocs: https://www.blm.gov/services/geospatial/GISData\nnote: |\n  BLM publishes no API authentication page, and the one machine-readable contract it serves\n  (the GBP Hub Search API) declares NO securitySchemes at all — because the public read surface\n  genuinely needs no credential. That is the headline for an agent: the entire public geospatial\n  surface is anonymous.\n\n  Credentials only appear on the two transactional systems, MLRS and GLO Records, which are\n  Salesforce Experience Cloud sites running on BLM's own hosts. Both serve a real OIDC\n  discovery document anonymously while every other path answers 401.\nsummary:\n  types: [none, oauth2, openIdConnect]\n  anonymous_read_surface:\
  \ true\n  api_key_in: []\n  oauth2_flows: [authorizationCode, implicit]\nschemes:\n  - name: anonymous\n    type: none\n    surface: GBP Hub Search API (OGC API - Records)\n    sources: [openapi/bureau-of-land-management-gbp-hub-search-openapi.json]\n    evidence: >-\n      The document declares no components.securitySchemes and no security[]. All 17 operations\n      were called anonymously on 2026-09-05 and returned 200. An optional `token` query\n      parameter exists on the item operations for reaching private ArcGIS items; it is not\n      required for BLM's public catalog.\n  - name: anonymous\n    type: none\n    surface: ArcGIS Server REST (13 instances on gis.blm.gov)\n    sources: [openapi/bureau-of-land-management-arcgis-service-inventory.json]\n    evidence: >-\n      Every /rest/info reports authInfo.isTokenBasedSecurity = false. Service directory, layer\n      metadata and /query were all exercised anonymously on 2026-09-05.\n  - name: anonymous\n    type: none\n    surface:\
  \ OGC WMS (gis.blm.gov/arcgis/services)\n    sources: [openapi/bureau-of-land-management-sma-wms-capabilities.xml]\n    evidence: >-\n      GetCapabilities returned HTTP 200 with no authentication on all seven services fetched.\n  - name: arcgis-online-oauth2\n    type: oauth2\n    surface: BLM ArcGIS Online organization (blm-egis.maps.arcgis.com)\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://blm-egis.maps.arcgis.com/sharing/rest/oauth2/authorize\n        tokenUrl: https://blm-egis.maps.arcgis.com/sharing/rest/oauth2/token\n        pkce: S256\n      - flow: implicit\n        authorizationUrl: https://blm-egis.maps.arcgis.com/sharing/rest/oauth2/authorize\n    sources: [well-known/bureau-of-land-management-blm-egis-arcgis-oauth-authorization-server.json]\n    evidence: >-\n      RFC 8414 metadata, HTTP 200, issuer https://blm-egis.maps.arcgis.com,\n      grant_types_supported [authorization_code, implicit],\n      code_challenge_methods_supported [\"S256\"\
  ]. Needed only to publish or reach non-public\n      items; BLM's published content is open.\n  - name: mlrs-oidc\n    type: openIdConnect\n    surface: Mineral and Land Records System (mlrs.blm.gov)\n    openIdConnectUrl: https://mlrs.blm.gov/.well-known/openid-configuration\n    issuer: https://mlrs.blm.gov\n    endpoints:\n      authorization: https://mlrs.blm.gov/services/oauth2/authorize\n      token: https://mlrs.blm.gov/services/oauth2/token\n      userinfo: https://mlrs.blm.gov/services/oauth2/userinfo\n      revocation: https://mlrs.blm.gov/services/oauth2/revoke\n      introspection: https://mlrs.blm.gov/services/oauth2/introspect\n      registration: https://mlrs.blm.gov/services/oauth2/register\n      jwks_uri: https://mlrs.blm.gov/id/keys\n      end_session: https://mlrs.blm.gov/services/auth/idp/oidc/logout\n    sources: [well-known/bureau-of-land-management-mlrs-openid-configuration.json]\n    evidence: >-\n      HTTP 200 anonymously on 2026-09-05. Every other probed path\
  \ on this host answered 401.\n      The 36 advertised scopes are the stock Salesforce platform scope set (api, web, openid,\n      refresh_token, cdp_*, pardot_api, ...), not a BLM-authored permission model — see\n      scopes/bureau-of-land-management-scopes.yml.\n  - name: glorecords-oidc\n    type: openIdConnect\n    surface: General Land Office Records (glorecords.blm.gov)\n    openIdConnectUrl: https://glorecords.blm.gov/.well-known/openid-configuration\n    issuer: https://glorecords.blm.gov\n    endpoints:\n      authorization: https://glorecords.blm.gov/services/oauth2/authorize\n      token: https://glorecords.blm.gov/services/oauth2/token\n      userinfo: https://glorecords.blm.gov/services/oauth2/userinfo\n      revocation: https://glorecords.blm.gov/services/oauth2/revoke\n      introspection: https://glorecords.blm.gov/services/oauth2/introspect\n      registration: https://glorecords.blm.gov/services/oauth2/register\n      jwks_uri: https://glorecords.blm.gov/id/keys\n  \
  \    end_session: https://glorecords.blm.gov/services/auth/idp/oidc/logout\n    sources: [well-known/bureau-of-land-management-glorecords-openid-configuration.json]\n    evidence: HTTP 200 anonymously on 2026-09-05; all other paths on this host answered 401.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bureau-of-land-management/refs/heads/main/authentication/bureau-of-land-management-authentication.yml
summary_line: none/oauth2/openIdConnect · 6 schemes
tags:
- Environment
- Federal-Government
- Land
- Resources
- GIS
- Geospatial
- Mining
- Public-Lands
- Open-Data
- OGC
- Cadastral
- Recreation
- Grazing
- ArcGIS
- DCAT
- Conservation
- Mapping
---
