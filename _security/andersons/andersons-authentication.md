---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: probed
name: Andersons Authentication
name_suffix: Authentication
oauth_flows: []
overview: The Andersons declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: The Andersons
provider_slug: andersons
scheme_count: 0
schemes: []
slug: andersons-authentication
source_filename: andersons-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-02'\nmethod: probed\nsource: https://portalauth.andersonsinc.com/adfs/.well-known/openid-configuration\ndocs: https://www.andersonsgrain.com/tools/grainweb/\nnote: >-\n  The Andersons publishes no public API and therefore no API authentication reference.\n  What it DOES publish, anonymously and machine-readably, is the OpenID Connect discovery\n  document for the Active Directory Federation Services deployment that authenticates its\n  customer-facing portals. This artifact records that federation surface exactly as the\n  provider serves it — it is identity infrastructure for GRAINweb, SmartTicket and the\n  account portal, NOT the auth model of a developer-facing API. Do not read it as evidence\n  that an API exists.\nscope: >-\n  Customer portal single sign-on (GRAINweb grain account portal, Farm2Market SmartTicket,\n  portal.andersonsinc.com account management). Client registration is not self-service and\n  is not documented publicly.\nissuer: https://portalauth.andersonsinc.com/adfs\n\
  protocols:\n  - id: openid-connect\n    version: OpenID Connect 1.0 (Microsoft ADFS)\n    discovery: https://portalauth.andersonsinc.com/adfs/.well-known/openid-configuration\n    status: 200\n  - id: oauth2\n    version: RFC 6749 / RFC 8628 device authorization\n    status: 200\n  - id: ws-federation\n    version: WS-Federation 1.2\n    evidence: >-\n      grainweb.com and andersonstickets.com both 302 to\n      https://portalauth.andersonsinc.com/adfs/ls/?wtrealm=...&wa=wsignin1.0\n    status: 200\n  - id: saml2\n    version: SAML 2.0\n    metadata: https://portalauth.andersonsinc.com/FederationMetadata/2007-06/FederationMetadata.xml\n    status: 200\n    note: 77KB signed SAML 2.0 EntityDescriptor, entityID http://portalauth.andersonsinc.com/adfs/services/trust\n  - id: ws-trust\n    version: WS-Trust 1.3\n    mex: https://portalauth.andersonsinc.com/adfs/services/trust/mex\n    status: 200\n    note: >-\n      Serves a live WSDL, but it is Microsoft's stock SecurityTokenService definition\n\
  \      (targetNamespace http://schemas.microsoft.com/ws/2008/06/identity/securitytokenservice),\n      not a contract The Andersons authored. Deliberately NOT saved to wsdl/ and NOT wired as\n      type WSDL — crediting it as a published SOAP contract would credit the company with an\n      API it did not ship.\nsecurity_schemes:\n  - type: openIdConnect\n    name: portalauth_adfs_oidc\n    openIdConnectUrl: https://portalauth.andersonsinc.com/adfs/.well-known/openid-configuration\n    in: header\n    scheme: bearer\n    bearer_format: JWT\n    id_token_signing_alg_values_supported:\n      - RS256\n    jwks_uri: https://portalauth.andersonsinc.com/adfs/discovery/keys\n  - type: oauth2\n    name: portalauth_adfs_oauth2\n    flows:\n      authorizationCode:\n        authorizationUrl: https://portalauth.andersonsinc.com/adfs/oauth2/authorize/\n        tokenUrl: https://portalauth.andersonsinc.com/adfs/oauth2/token/\n        refreshUrl: https://portalauth.andersonsinc.com/adfs/oauth2/token/\n\
  \      clientCredentials:\n        tokenUrl: https://portalauth.andersonsinc.com/adfs/oauth2/token/\n      deviceCode:\n        deviceAuthorizationUrl: https://portalauth.andersonsinc.com/adfs/oauth2/devicecode\n        tokenUrl: https://portalauth.andersonsinc.com/adfs/oauth2/token/\n      implicit:\n        authorizationUrl: https://portalauth.andersonsinc.com/adfs/oauth2/authorize/\n        note: Advertised by the discovery document; deprecated by current OAuth guidance.\n      password:\n        tokenUrl: https://portalauth.andersonsinc.com/adfs/oauth2/token/\n        note: Advertised by the discovery document; deprecated by current OAuth guidance.\ngrant_types_supported:\n  - authorization_code\n  - refresh_token\n  - client_credentials\n  - urn:ietf:params:oauth:grant-type:jwt-bearer\n  - implicit\n  - password\n  - srv_challenge\n  - urn:ietf:params:oauth:grant-type:device_code\n  - device_code\ntoken_endpoint_auth_methods_supported:\n  - client_secret_post\n  - client_secret_basic\n\
  \  - private_key_jwt\n  - windows_client_authentication\nresponse_types_supported:\n  - code\n  - id_token\n  - code id_token\n  - id_token token\n  - code token\n  - code id_token token\nendpoints:\n  authorization: https://portalauth.andersonsinc.com/adfs/oauth2/authorize/\n  token: https://portalauth.andersonsinc.com/adfs/oauth2/token/\n  userinfo: https://portalauth.andersonsinc.com/adfs/userinfo\n  jwks: https://portalauth.andersonsinc.com/adfs/discovery/keys\n  end_session: https://portalauth.andersonsinc.com/adfs/oauth2/logout\n  device_authorization: https://portalauth.andersonsinc.com/adfs/oauth2/devicecode\nfeatures:\n  pkce_documented: false\n  dynamic_client_registration: false\n  front_channel_logout: true\n  token_binding: true\n  subject_types_supported:\n    - pairwise\ngaps:\n  - No public developer client registration; no documented way for a third party to obtain a client_id.\n  - No /.well-known/oauth-protected-resource (RFC 9728) — 503 on this host.\n  - PKCE is not\
  \ advertised in the discovery document (code_challenge_methods_supported absent).\n  - No API bound to this issuer is publicly documented, so the token has no published audience.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/andersons/refs/heads/main/authentication/andersons-authentication.yml
summary_line: 0 schemes
tags:
- Agribusiness
- Agriculture
- Grain
- Commodity Merchandising
- Plant Nutrients
- Fertilizer
- Renewables
- Ethanol
- Food and Feed Ingredients
- Turf and Specialty Products
- Rail Leasing
- Supply Chain
---
