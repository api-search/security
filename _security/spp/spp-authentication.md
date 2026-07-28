---
api_key_in:
- query
api_specs:
- filename: trolie-standard-openapi.yml
  format: yaml
  label: SPP LEP/TROLIE Ratings API
  slug: spp-lep-trolie-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spp/refs/heads/main/openapi/trolie-standard-openapi.yml
auth_types:
- none
- apiKey
- mutualTLS
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
method: searched
name: Spp Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Southwest Power Pool secures its APIs with none, apiKey, mutualTLS, oauth2, and openIdConnect across 5 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Southwest Power Pool
provider_slug: spp
scheme_count: 5
schemes:
- applies_to:
  - spp:spp-public-data-ftp
  - spp:spp-portal-file-browser-api
  - spp:spp-portal-chart-api
  description: No authentication. Verified anonymously on 2026-07-27 against ftp://pubftp.spp.org (FTP 226), portal.spp.org/file-browser-api/download (HTTP 200, text/csv), portal.spp.org/chart-api (HTTP 200, application/json) and pricecontourmap.spp.org/arcgis/rest/services (HTTP 200, application/json). No account, key, token, cookie or licence click-through is enforced in the request path.
  name: anonymous-public-data
  sources:
  - probe
  type: none
- applies_to:
  - spp:spp-price-contour-map-arcgis
  description: The ArcGIS Server behind the price contour map advertises token-based security in its own service-info document — /arcgis/rest/info?f=json returns isTokenBasedSecurity true with tokenServicesUrl https://pricecontourmap.spp.org/arcgis/tokens/. The PCM folder services are nonetheless readable anonymously; the token service governs privileged operations. This is the standard Esri ArcGIS REST contract, not an SPP-authored scheme.
  evidence: examples/spp-arcgis-rest-info.json
  in: query
  name: arcgis-token
  parameter: token
  sources:
  - probe
  type: apiKey
- applies_to:
  - spp:spp-lep-trolie-api
  - spp:spp-integrated-marketplace-web-services
  description: 'Two-factor: an x.509 client certificate issued by a CA SPP trusts, presented over mTLS, plus an SPP UAA identity whose roles and scope authorize the function. SPP''s "Digital Certificates and the Integrated Marketplace" document states OATI webCARES is the Certificate Authority trusted by Integrated Marketplace applications. SPP''s System Interfaces Stakeholder Reference Guide (v1.0, 2025-01-29) states most programmatic services require two-factor authentication. The SPP LEP/TROLIE API Data Exchange Guide (v1.0, 2024-11-08) describes UAA authenticating the certificate and then looking up the user''s roles and scope per connection. Access is provisioned by a Local Security Administrator and requested through an RMS ticket.'
  name: oati-webcares-x509-plus-uaa
  sources:
  - https://www.spp.org/documents/18307/digital%20certificates%20and%20the%20integrated%20marketplace%20doc_final.pdf
  - https://www.spp.org/documents/73131/spp%20system%20interfaces%20stakeholder%20reference%20guide%2020250129.pdf
  - https://www.spp.org/documents/72496/spp%20lep%20api%20data%20exchange%20guide.pdf
  type: mutualTLS
- applies_to:
  - spp:spp-lep-trolie-api
  description: 'Declared by the LF Energy TROLIE community specification (the contract SPP''s LEP guide directs implementers to), not by an SPP-hosted authorization server. clientCredentials flow with 15 read:/write: scopes and RFC 8725 JWT token guidance. The spec''s tokenUrl is relative to its placeholder server host, so no real SPP token endpoint can be derived from it.'
  flows:
  - flow: clientCredentials
    scopes: 15
    tokenUrl: relative /oauth2 against the spec placeholder server (no SPP host published)
  name: oauth2-primary-flow
  scopes_artifact: scopes/spp-scopes.yml
  sources:
  - openapi/trolie-standard-openapi.yml
  standard_scheme: true
  type: oauth2
- description: OIDC discovery document served anonymously by SPP's Request Management System (Salesforce Experience Cloud). issuer https://rms.spp.org, authorize /services/oauth2/authorize, token /services/oauth2/token, jwks /id/keys, RS256, PKCE S256, dynamic client registration advertised. Governs access to the ticketing system a stakeholder uses to request API access — it is not the authorization server for any SPP data or market API.
  evidence: well-known/spp-rms-openid-configuration.json
  name: rms-openid-connect
  openIdConnectUrl: https://rms.spp.org/.well-known/openid-configuration
  sources:
  - probe
  type: openIdConnect
slug: spp-authentication
source_filename: spp-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-27'\nmethod: searched\nsource: openapi/trolie-standard-openapi.yml\ndocs: https://www.spp.org/documents/18307/digital%20certificates%20and%20the%20integrated%20marketplace%20doc_final.pdf\nnote: >-\n  SPP runs two completely different authentication regimes. Everything a\n  developer can reach anonymously — the public data FTP site, the SPP Portal\n  file-browser and chart download paths, and the price-contour ArcGIS REST\n  services — requires no credential at all. Everything a market participant\n  transacts against requires an x.509 digital certificate from a Certificate\n  Authority SPP trusts (OATI webCARES for Integrated Marketplace applications)\n  presented over mTLS, plus an identity in SPP UAA whose assigned roles and\n  scope authorize the specific function. SPP publishes no OAuth authorization\n  server, no OpenID Connect discovery document and no API key issuance for those\n  APIs. The only OIDC discovery document served anywhere on an SPP host\
  \ is for\n  rms.spp.org, the Salesforce-hosted Request Management System used to request\n  access — not an API authorization server.\nsummary:\n  types: [none, apiKey, mutualTLS, oauth2, openIdConnect]\n  api_key_in: [query]\n  oauth2_flows: [clientCredentials]\n  anonymous_surfaces: 4\n  gated_surfaces: 2\nschemes:\n- name: anonymous-public-data\n  type: none\n  description: >-\n    No authentication. Verified anonymously on 2026-07-27 against\n    ftp://pubftp.spp.org (FTP 226), portal.spp.org/file-browser-api/download\n    (HTTP 200, text/csv), portal.spp.org/chart-api (HTTP 200, application/json)\n    and pricecontourmap.spp.org/arcgis/rest/services (HTTP 200, application/json).\n    No account, key, token, cookie or licence click-through is enforced in the\n    request path.\n  applies_to:\n  - spp:spp-public-data-ftp\n  - spp:spp-portal-file-browser-api\n  - spp:spp-portal-chart-api\n  sources: [probe]\n- name: arcgis-token\n  type: apiKey\n  in: query\n  parameter: token\n  description:\
  \ >-\n    The ArcGIS Server behind the price contour map advertises token-based\n    security in its own service-info document — /arcgis/rest/info?f=json returns\n    isTokenBasedSecurity true with tokenServicesUrl\n    https://pricecontourmap.spp.org/arcgis/tokens/. The PCM folder services are\n    nonetheless readable anonymously; the token service governs privileged\n    operations. This is the standard Esri ArcGIS REST contract, not an\n    SPP-authored scheme.\n  applies_to: [spp:spp-price-contour-map-arcgis]\n  evidence: examples/spp-arcgis-rest-info.json\n  sources: [probe]\n- name: oati-webcares-x509-plus-uaa\n  type: mutualTLS\n  description: >-\n    Two-factor: an x.509 client certificate issued by a CA SPP trusts, presented\n    over mTLS, plus an SPP UAA identity whose roles and scope authorize the\n    function. SPP's \"Digital Certificates and the Integrated Marketplace\"\n    document states OATI webCARES is the Certificate Authority trusted by\n    Integrated Marketplace\
  \ applications. SPP's System Interfaces Stakeholder\n    Reference Guide (v1.0, 2025-01-29) states most programmatic services require\n    two-factor authentication. The SPP LEP/TROLIE API Data Exchange Guide (v1.0,\n    2024-11-08) describes UAA authenticating the certificate and then looking up\n    the user's roles and scope per connection. Access is provisioned by a Local\n    Security Administrator and requested through an RMS ticket.\n  applies_to:\n  - spp:spp-lep-trolie-api\n  - spp:spp-integrated-marketplace-web-services\n  sources:\n  - https://www.spp.org/documents/18307/digital%20certificates%20and%20the%20integrated%20marketplace%20doc_final.pdf\n  - https://www.spp.org/documents/73131/spp%20system%20interfaces%20stakeholder%20reference%20guide%2020250129.pdf\n  - https://www.spp.org/documents/72496/spp%20lep%20api%20data%20exchange%20guide.pdf\n- name: oauth2-primary-flow\n  type: oauth2\n  standard_scheme: true\n  description: >-\n    Declared by the LF Energy TROLIE community\
  \ specification (the contract SPP's\n    LEP guide directs implementers to), not by an SPP-hosted authorization\n    server. clientCredentials flow with 15 read:/write: scopes and RFC 8725 JWT\n    token guidance. The spec's tokenUrl is relative to its placeholder server\n    host, so no real SPP token endpoint can be derived from it.\n  flows:\n  - flow: clientCredentials\n    tokenUrl: relative /oauth2 against the spec placeholder server (no SPP host published)\n    scopes: 15\n  applies_to: [spp:spp-lep-trolie-api]\n  sources: [openapi/trolie-standard-openapi.yml]\n  scopes_artifact: scopes/spp-scopes.yml\n- name: rms-openid-connect\n  type: openIdConnect\n  openIdConnectUrl: https://rms.spp.org/.well-known/openid-configuration\n  description: >-\n    OIDC discovery document served anonymously by SPP's Request Management\n    System (Salesforce Experience Cloud). issuer https://rms.spp.org, authorize\n    /services/oauth2/authorize, token /services/oauth2/token, jwks /id/keys,\n   \
  \ RS256, PKCE S256, dynamic client registration advertised. Governs access to\n    the ticketing system a stakeholder uses to request API access — it is not\n    the authorization server for any SPP data or market API.\n  evidence: well-known/spp-rms-openid-configuration.json\n  sources: [probe]\nnot_found:\n- API key issuance or developer key management of any kind\n- OAuth authorization server or OIDC discovery for any SPP data or market API\n- self-serve developer registration\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/spp/refs/heads/main/authentication/spp-authentication.yml
summary_line: none/apiKey/mutualTLS/oauth2/openIdConnect · 5 schemes
tags:
- Energy
- United States
- Energy Markets
- Electricity
- Grid
- Utilities
- Renewables
- Market Data
- Transmission
- System Operator
---
