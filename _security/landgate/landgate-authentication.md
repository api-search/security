---
api_key_in: []
api_specs:
- filename: landgate-datasets-api-openapi.yml
  format: yaml
  label: Landgate Datasets API
  slug: landgate-datasets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/landgate/refs/heads/main/openapi/landgate-datasets-api-openapi.yml
- filename: landgate-discovery-api-openapi.yml
  format: yaml
  label: Landgate Discovery API
  slug: landgate-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/landgate/refs/heads/main/openapi/landgate-discovery-api-openapi.yml
- filename: landgate-organizations-api-openapi.yml
  format: yaml
  label: Landgate Organizations API
  slug: landgate-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/landgate/refs/heads/main/openapi/landgate-organizations-api-openapi.yml
- filename: landgate-query-api-openapi.yml
  format: yaml
  label: Landgate Query API
  slug: landgate-query-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/landgate/refs/heads/main/openapi/landgate-query-api-openapi.yml
- filename: landgate-server-api-openapi.yml
  format: yaml
  label: Landgate Server API
  slug: landgate-server-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/landgate/refs/heads/main/openapi/landgate-server-api-openapi.yml
- filename: landgate-services-api-openapi.yml
  format: yaml
  label: Landgate Services API
  slug: landgate-services-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/landgate/refs/heads/main/openapi/landgate-services-api-openapi.yml
- filename: landgate-site-api-openapi.yml
  format: yaml
  label: Landgate Site API
  slug: landgate-site-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/landgate/refs/heads/main/openapi/landgate-site-api-openapi.yml
- filename: landgate-wfs-api-openapi.yml
  format: yaml
  label: Landgate WFS API
  slug: landgate-wfs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/landgate/refs/heads/main/openapi/landgate-wfs-api-openapi.yml
- filename: landgate-wms-api-openapi.yml
  format: yaml
  label: Landgate WMS API
  slug: landgate-wms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/landgate/refs/heads/main/openapi/landgate-wms-api-openapi.yml
auth_types:
- none
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
method: searched
name: Landgate Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- implicit
- clientCredentials
- refreshToken
- deviceCode
- tokenExchange
- jwtBearer
- saml2Bearer
- ciba
- password
overview: Landgate secures its APIs with none, oauth2, and openIdConnect across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode, implicit, clientCredentials, refreshToken, deviceCode, tokenExchange, jwtBearer, saml2Bearer, ciba, and password flow(s).
provider_name: Landgate
provider_slug: landgate
scheme_count: 2
schemes:
- issuer: https://sign-on.app.landgate.wa.gov.au
  name: MyLandgateOIDC
  openIdConnectUrl: https://sign-on.app.landgate.wa.gov.au/.well-known/openid-configuration
  product: PingFederate
  sources:
  - well-known/landgate-openid-configuration.json
  - openapi/landgate-mylandgate-openid-configuration.json
  type: openIdConnect
- endpoints:
    end_session: https://sign-on.app.landgate.wa.gov.au/idp/init_logout.openid
    introspection: https://sign-on.app.landgate.wa.gov.au/as/introspect.oauth2
    jwks: https://sign-on.app.landgate.wa.gov.au/pf/JWKS
    registration: https://sign-on.app.landgate.wa.gov.au/as/clients.oauth2
    revocation: https://sign-on.app.landgate.wa.gov.au/as/revoke_token.oauth2
    token: https://sign-on.app.landgate.wa.gov.au/as/token.oauth2
    userinfo: https://sign-on.app.landgate.wa.gov.au/idp/userinfo.openid
  flows:
  - authorizationUrl: https://sign-on.app.landgate.wa.gov.au/as/authorization.oauth2
    flow: authorizationCode
    scopes:
    - openid
    - profile
    - email
    - address
    - phone
    - ATO
    tokenUrl: https://sign-on.app.landgate.wa.gov.au/as/token.oauth2
  - authorizationUrl: https://sign-on.app.landgate.wa.gov.au/as/authorization.oauth2
    flow: implicit
  - flow: clientCredentials
    tokenUrl: https://sign-on.app.landgate.wa.gov.au/as/token.oauth2
  - deviceAuthorizationUrl: https://sign-on.app.landgate.wa.gov.au/as/device_authz.oauth2
    flow: deviceCode
  metadata: RFC 8414 OAuth 2.0 Authorization Server Metadata
  name: MyLandgateOAuth2
  note: 'A registration_endpoint is advertised but this is the standard PingFederate dynamic

    client registration URL — no public developer flow, documentation or onboarding page was

    found for it. Treat the identity surface as staff/subscriber sign-on, not a developer API.

    '
  sources:
  - well-known/landgate-oauth-authorization-server.json
  token_endpoint_auth_methods:
  - client_secret_basic
  - client_secret_post
  - client_secret_jwt
  - private_key_jwt
  - tls_client_auth
  - none
  type: oauth2
slug: landgate-authentication
source_filename: landgate-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-26'\nmethod: searched\nsource: live probes of the SLIP public services, the Data WA CKAN catalogue and the\n  MyLandgate PingFederate discovery documents\ndocs: https://www.landgate.wa.gov.au/location-data-and-services/discovering-landgate-data/licensing/\nnote: |\n  Landgate's authentication story is split three ways and the split is the whole finding.\n  The public tier takes NO credential at all; the subscription tier takes a credential that\n  cannot be self-issued (it is granted after a licence is signed); and the identity provider\n  that fronts the gated tier is a real, standards-compliant OAuth 2.0 / OIDC authorization\n  server that publishes no public client registration path.\nsummary:\n  types: [none, oauth2, openIdConnect]\n  api_key_in: []\n  oauth2_flows: [authorizationCode, implicit, clientCredentials, refreshToken, deviceCode,\n    tokenExchange, jwtBearer, saml2Bearer, ciba, password]\n  self_service_signup: false\n  public_client_registration:\
  \ false\nsurfaces:\n  - name: SLIP Public Services (ArcGIS REST)\n    base: https://public-services.slip.wa.gov.au/public/rest\n    auth: none\n    evidence:\n      url: https://public-services.slip.wa.gov.au/public/rest/info?f=json\n      status: 200\n      probed: '2026-07-26'\n      body: '{\"authInfo\":{\"isTokenBasedSecurity\":false}}'\n    note: Confirmed anonymous — a live feature query returned real LGA boundary features\n      with no credential.\n  - name: SLIP Public OGC Services (WMS / WFS)\n    base: https://public-services.slip.wa.gov.au/public/services\n    auth: none\n    evidence:\n      url: https://public-services.slip.wa.gov.au/public/services/SLIP_Public_Services/Boundaries/MapServer/WMSServer?request=GetCapabilities&service=WMS\n      status: 200\n      probed: '2026-07-26'\n  - name: Data WA CKAN Action API\n    base: https://catalogue.data.wa.gov.au/api/3/action\n    auth: none (read)\n    evidence:\n      url: https://catalogue.data.wa.gov.au/api/3/action/status_show\n\
  \      status: 200\n      probed: '2026-07-26'\n    note: |\n      Read actions are anonymous. CKAN write actions require an API key sent in the\n      `Authorization` header, but Data WA issues no public API keys — no self-service key\n      surface was found. Do not record an apiKey scheme for the public surface.\n  - name: SLIP Subscription Services (ArcGIS REST)\n    base: https://services.slip.wa.gov.au/arcgis/rest/services\n    auth: gated\n    evidence:\n      url: https://services.slip.wa.gov.au/arcgis/rest/services\n      status: 401\n      probed: '2026-07-26'\n    note: HTTP 401 anonymously — even /arcgis/rest/info is 401. Access follows a signed SLIP\n      subscription / publication / broker / distributor / value-added-reseller licence.\n  - name: MyLandgate / Land Enquiry Services\n    base: https://sign-on.app.landgate.wa.gov.au\n    auth: oauth2 + openIdConnect\n    evidence:\n      url: https://sign-on.app.landgate.wa.gov.au/.well-known/openid-configuration\n      status:\
  \ 200\n      probed: '2026-07-26'\nschemes:\n  - name: MyLandgateOIDC\n    type: openIdConnect\n    openIdConnectUrl: https://sign-on.app.landgate.wa.gov.au/.well-known/openid-configuration\n    issuer: https://sign-on.app.landgate.wa.gov.au\n    product: PingFederate\n    sources:\n      - well-known/landgate-openid-configuration.json\n      - openapi/landgate-mylandgate-openid-configuration.json\n  - name: MyLandgateOAuth2\n    type: oauth2\n    sources: [well-known/landgate-oauth-authorization-server.json]\n    metadata: RFC 8414 OAuth 2.0 Authorization Server Metadata\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://sign-on.app.landgate.wa.gov.au/as/authorization.oauth2\n        tokenUrl: https://sign-on.app.landgate.wa.gov.au/as/token.oauth2\n        scopes: [openid, profile, email, address, phone, ATO]\n      - flow: implicit\n        authorizationUrl: https://sign-on.app.landgate.wa.gov.au/as/authorization.oauth2\n      - flow: clientCredentials\n\
  \        tokenUrl: https://sign-on.app.landgate.wa.gov.au/as/token.oauth2\n      - flow: deviceCode\n        deviceAuthorizationUrl: https://sign-on.app.landgate.wa.gov.au/as/device_authz.oauth2\n    endpoints:\n      token: https://sign-on.app.landgate.wa.gov.au/as/token.oauth2\n      revocation: https://sign-on.app.landgate.wa.gov.au/as/revoke_token.oauth2\n      introspection: https://sign-on.app.landgate.wa.gov.au/as/introspect.oauth2\n      userinfo: https://sign-on.app.landgate.wa.gov.au/idp/userinfo.openid\n      jwks: https://sign-on.app.landgate.wa.gov.au/pf/JWKS\n      registration: https://sign-on.app.landgate.wa.gov.au/as/clients.oauth2\n      end_session: https://sign-on.app.landgate.wa.gov.au/idp/init_logout.openid\n    token_endpoint_auth_methods: [client_secret_basic, client_secret_post, client_secret_jwt,\n      private_key_jwt, tls_client_auth, none]\n    note: |\n      A registration_endpoint is advertised but this is the standard PingFederate dynamic\n      client registration\
  \ URL — no public developer flow, documentation or onboarding page was\n      found for it. Treat the identity surface as staff/subscriber sign-on, not a developer API.\nonboarding:\n  self_service: false\n  api_key_issuance: none found\n  gate: signed licence (SLIP subscription / publication / broker / distributor / VAR) plus a\n    MyLandgate account for bulk downloads\n  contact: https://www.landgate.wa.gov.au/help-centre/\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/landgate/refs/heads/main/authentication/landgate-authentication.yml
summary_line: none/oauth2/openIdConnect · 2 schemes
tags:
- Real-Estate
- Australia
- Land Registry
- Title
- Valuation
- Property Data
- Open Data
- Geospatial
- Government
- Conveyancing
- PropTech
---
