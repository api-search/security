---
anonymous_access: true
api_key_in:
- query
auth_types:
- none
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: probed
name: Rayonier Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Rayonier secures its APIs with none, apiKey, and oauth2 across 4 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Rayonier
provider_slug: rayonier
scheme_count: 4
schemes:
- evidence: All 45 services in Public/ and Hosted/ returned their service document (HTTP 200) with no credential on 2026-09-17, and Public/Rayonier_FEE_Ownership_Public/FeatureServer/0/query?where=1%3D1&returnCountOnly=true returned {"count":6216} anonymously.
  name: anonymous
  sources:
  - arcgis/rayonier-arcgis-service-inventory.json
  surface: ArcGIS Server REST — Public and Hosted folders (gis.rayonier.com/arcgis/rest/services)
  type: none
- evidence: ?wsdl returned the 290 KB MapServer contract (HTTP 200, text/xml) with no credential on three Public/ services.
  name: anonymous
  sources:
  - wsdl/rayonier-fee-ownership-mapserver.wsdl
  surface: ArcGIS Server SOAP (gis.rayonier.com/arcgis/services)
  type: none
- evidence: /arcgis/rest/info reports authInfo.isTokenBasedSecurity true and names the token service; /arcgis/rest/services/Utilities?f=json answered {"error":{"code":499,"message":"Token Required"}}. Tokens are issued only to portal accounts; signup is disabled.
  in: query
  name: arcgis-token
  param: token
  surface: ArcGIS Server REST — Utilities folder and any non-public item
  tokenUrl: https://gis.rayonier.com/portal/sharing/rest/generateToken
  type: apiKey
- evidence: 'portals/self reports supportsOAuth true and samlEnabled true; /portal/sharing/login 302s to /portal/sharing/oauth2/authorize?client_id=arcgisonline&response_type=code. No RFC 8414 /.well-known/oauth-authorization-server document is served (404), and no scope list is published, so scopes: is empty rather than guessed. Staff-only: disableSignup is true.'
  flows:
  - authorizationUrl: https://gis.rayonier.com/portal/sharing/rest/oauth2/authorize
    flow: authorizationCode
    scopes: {}
    tokenUrl: https://gis.rayonier.com/portal/sharing/rest/oauth2/token
  name: portal-oauth2
  surface: Portal for ArcGIS (gis.rayonier.com/portal)
  type: oauth2
slug: rayonier-authentication
source_filename: rayonier-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-17'\nmethod: probed\nsource: >-\n  https://gis.rayonier.com/arcgis/rest/info?f=json (saved as arcgis/rayonier-arcgis-rest-info.json),\n  https://gis.rayonier.com/portal/sharing/rest/portals/self?f=json (saved as\n  arcgis/rayonier-arcgis-portal-self.json), and anonymous calls against the Public and Hosted\n  service folders, 2026-09-17.\ndocs: null\nnote: |\n  Rayonier publishes no authentication page and no developer documentation of any kind. What is\n  recorded here was read out of the server's own discovery documents and confirmed by calling\n  the surface anonymously. The headline for an agent: every service in the Public and Hosted\n  folders (45 services, 102 layers) answers metadata and /query calls with NO credential. The\n  Utilities folder is the one place a token is demanded — it returned the ArcGIS error envelope\n  {\"error\":{\"code\":499,\"message\":\"Token Required\"}}.\n\n  The server itself runs token-based security (authInfo.isTokenBasedSecurity\
  \ = true, tokens\n  minted at the portal's generateToken endpoint) and the portal supports OAuth 2.0 and SAML\n  (supportsOAuth = true, samlEnabled = true, disableSignup = true). Those are the credentials\n  Rayonier staff use to reach non-public items; the sign-in page redirects to\n  /portal/sharing/oauth2/authorize with client_id=arcgisonline. Self-signup is disabled, so\n  there is no path for an outside developer to obtain a token — the public surface is the\n  whole public surface.\n\n  No write was attempted. Nine services ADVERTISE Create/Update/Delete in their capabilities\n  string (see conventions/); whether an anonymous caller can exercise them was deliberately not\n  tested.\nsummary:\n  types: [none, apiKey, oauth2]\n  anonymous_read_surface: true\n  api_key_in: [query]\n  oauth2_flows: [authorizationCode]\n  self_signup: false\nschemes:\n  - name: anonymous\n    type: none\n    surface: ArcGIS Server REST — Public and Hosted folders (gis.rayonier.com/arcgis/rest/services)\n\
  \    sources: [arcgis/rayonier-arcgis-service-inventory.json]\n    evidence: >-\n      All 45 services in Public/ and Hosted/ returned their service document (HTTP 200) with no\n      credential on 2026-09-17, and\n      Public/Rayonier_FEE_Ownership_Public/FeatureServer/0/query?where=1%3D1&returnCountOnly=true\n      returned {\"count\":6216} anonymously.\n  - name: anonymous\n    type: none\n    surface: ArcGIS Server SOAP (gis.rayonier.com/arcgis/services)\n    sources: [wsdl/rayonier-fee-ownership-mapserver.wsdl]\n    evidence: >-\n      ?wsdl returned the 290 KB MapServer contract (HTTP 200, text/xml) with no credential on\n      three Public/ services.\n  - name: arcgis-token\n    type: apiKey\n    in: query\n    param: token\n    surface: ArcGIS Server REST — Utilities folder and any non-public item\n    tokenUrl: https://gis.rayonier.com/portal/sharing/rest/generateToken\n    evidence: >-\n      /arcgis/rest/info reports authInfo.isTokenBasedSecurity true and names the token service;\n\
  \      /arcgis/rest/services/Utilities?f=json answered {\"error\":{\"code\":499,\"message\":\"Token\n      Required\"}}. Tokens are issued only to portal accounts; signup is disabled.\n  - name: portal-oauth2\n    type: oauth2\n    surface: Portal for ArcGIS (gis.rayonier.com/portal)\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://gis.rayonier.com/portal/sharing/rest/oauth2/authorize\n        tokenUrl: https://gis.rayonier.com/portal/sharing/rest/oauth2/token\n        scopes: {}\n    evidence: >-\n      portals/self reports supportsOAuth true and samlEnabled true; /portal/sharing/login 302s\n      to /portal/sharing/oauth2/authorize?client_id=arcgisonline&response_type=code. No\n      RFC 8414 /.well-known/oauth-authorization-server document is served (404), and no scope\n      list is published, so scopes: is empty rather than guessed. Staff-only: disableSignup is\n      true.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rayonier/refs/heads/main/authentication/rayonier-authentication.yml
summary_line: none/apiKey/oauth2 · 4 schemes
tags:
- Timber
- Real Estate
- Forest Products
- Geospatial
- ArcGIS REST
- Land Management
- Hunting Leases
- Forestry
---
