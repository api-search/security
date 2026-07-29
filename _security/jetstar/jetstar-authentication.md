---
api_key_in: []
auth_types:
- mutualTLS
- session-token
- ip-allowlist
description: 'The Jetstar API is a Navitaire New Skies (NSK 4.6) SOAP/WCF web service, not a REST product. Authentication is therefore not an OpenAPI securityScheme: it is a three-layer gate — transport-level mutual TLS with a Jetstar-issued client certificate, network-level source-IP allow-listing, and an application-level Navitaire session Signature that is obtained by a logon call and then carried on every subsequent request. Before any of that, a caller must be an IATA-accredited Jetstar Registered Travel Agent with separate Jetstar approval for API access.'
kind: authentication
layout: security
method: searched
name: Jetstar Authentication
name_suffix: Authentication
oauth_flows: []
overview: Jetstar secures its APIs with mutualTLS, session-token, and ip-allowlist across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Jetstar
provider_slug: jetstar
scheme_count: 3
schemes:
- description: Jetstar issues a client SSL certificate to each approved partner and publishes a certificate installation manual in the gated Download Centre. Connections presenting no certificate are refused.
  evidence: Portal Download Centre lists a client-certificate installation manual; https://jqapi.navitaire.com times out for non-certificated clients.
  layer: transport
  name: ClientCertificate
  source: https://apiblog.jetstar.com/faq/
  type: mutualTLS
- description: Calling IP addresses must be registered with Jetstar and allow-listed. Jetstar's connection-issue guidance is written around "update IP address".
  evidence: Partner FAQ connection-troubleshooting guidance.
  layer: network
  name: SourceIPAllowList
  source: https://apiblog.jetstar.com/faq/
  type: network
- description: Navitaire New Skies issues a session Signature that is passed on every subsequent SOAP request. Sessions expire after 20 minutes of inactivity and must be re-established.
  evidence: Partner FAQ documents the session Signature and the 20-minute session timeout; C# request objects (GetStationListRequest / GetStationListRequestData) carry the signature.
  in: soap-message
  layer: application
  name: NavitaireSessionSignature
  parameter_name: Signature
  session_timeout_minutes: 20
  source: https://apiblog.jetstar.com/faq/
  type: session-token
slug: jetstar-authentication
source_filename: jetstar-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-28'\nmethod: searched\nsource: >-\n  https://apiblog.jetstar.com/faq/ (read via the portal's publicly readable\n  WordPress REST API, page id 6) and https://apiblog.jetstar.com/where-we-fly/.\n  No OpenAPI or WSDL is published, so nothing was derived mechanically —\n  0-working/derive-authentication.py has no spec to read for this provider.\ndocs: https://apiblog.jetstar.com/faq/\ndescription: >-\n  The Jetstar API is a Navitaire New Skies (NSK 4.6) SOAP/WCF web service, not a\n  REST product. Authentication is therefore not an OpenAPI securityScheme: it is\n  a three-layer gate — transport-level mutual TLS with a Jetstar-issued client\n  certificate, network-level source-IP allow-listing, and an application-level\n  Navitaire session Signature that is obtained by a logon call and then carried\n  on every subsequent request. Before any of that, a caller must be an\n  IATA-accredited Jetstar Registered Travel Agent with separate Jetstar approval\n  for API\
  \ access.\n\nsummary:\n  types:\n    - mutualTLS\n    - session-token\n    - ip-allowlist\n  api_key_in: []\n  oauth2_flows: []\n  oauth2: false\n  oidc: false\n  self_serve_credentials: false\n\nschemes:\n  - name: ClientCertificate\n    type: mutualTLS\n    layer: transport\n    description: >-\n      Jetstar issues a client SSL certificate to each approved partner and\n      publishes a certificate installation manual in the gated Download Centre.\n      Connections presenting no certificate are refused.\n    evidence: >-\n      Portal Download Centre lists a client-certificate installation manual;\n      https://jqapi.navitaire.com times out for non-certificated clients.\n    source: https://apiblog.jetstar.com/faq/\n  - name: SourceIPAllowList\n    type: network\n    layer: network\n    description: >-\n      Calling IP addresses must be registered with Jetstar and allow-listed.\n      Jetstar's connection-issue guidance is written around \"update IP address\".\n    evidence: Partner\
  \ FAQ connection-troubleshooting guidance.\n    source: https://apiblog.jetstar.com/faq/\n  - name: NavitaireSessionSignature\n    type: session-token\n    layer: application\n    in: soap-message\n    parameter_name: Signature\n    description: >-\n      Navitaire New Skies issues a session Signature that is passed on every\n      subsequent SOAP request. Sessions expire after 20 minutes of inactivity\n      and must be re-established.\n    session_timeout_minutes: 20\n    evidence: >-\n      Partner FAQ documents the session Signature and the 20-minute session\n      timeout; C# request objects (GetStationListRequest /\n      GetStationListRequestData) carry the signature.\n    source: https://apiblog.jetstar.com/faq/\n\nnot_supported:\n  - id: oauth2\n    note: No OAuth 2.0 authorization server, no token endpoint, no scopes. scopes/ is intentionally absent.\n  - id: openIdConnect\n    note: No /.well-known/openid-configuration on any Jetstar or Navitaire host.\n  - id: apiKey\n    note:\
  \ No self-serve API key; credentials are issued per approved partner.\n\nonboarding:\n  self_serve: false\n  public_signup: false\n  registration_url: https://apiblog.jetstar.com/api-registration/\n  prerequisites:\n    - Jetstar Registered Travel Agent status under the Jetstar Travel Agent Terms and Conditions\n    - IATA GoStandard or GoGlobal accreditation for BSP settlement (GoLite unsupported since 4 December 2023)\n    - Separate Jetstar approval specifically for API access\n    - Portal login at apiblog.jetstar.com for documentation and the Download Centre\n    - Installed client SSL certificate and allow-listed calling IP addresses\n  support_contact: apisupport@jetstar.com\n\nenvironments:\n  - name: production\n    version: NSK 4.6\n    url: https://jqapi.navitaire.com\n  - name: test\n    version: NSK 4.6\n    url: https://soapapir4y.test.jq.navitaire.com\n\nrelated:\n  conventions: conventions/jetstar-conventions.yml\n  sandbox: sandbox/jetstar-sandbox.yml\n  lifecycle: lifecycle/jetstar-lifecycle.yml\n\
  \  conformance: conformance/jetstar-conformance.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/jetstar/refs/heads/main/authentication/jetstar-authentication.yml
summary_line: mutualTLS/session-token/ip-allowlist · 3 schemes
tags:
- Travel
- Australia
- Aviation
- Airline
- Low Cost Carrier
- Distribution
- Booking
- GDS
- Corporate Travel
- Qantas Group
---
