---
api_key_in: []
api_specs:
- filename: rightmove-commercial-listings-openapi.yml
  format: yaml
  label: Rightmove Commercial Listings API
  slug: rightmove-commercial-listings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rightmove/refs/heads/main/openapi/rightmove-commercial-listings-openapi.yml
auth_types:
- oauth2
- mutualTLS
description: ''
kind: authentication
layout: security
method: searched
name: Rightmove Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Rightmove secures its APIs with oauth2 and mutualTLS across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Rightmove
provider_slug: rightmove
scheme_count: 2
schemes:
- additional_headers:
  - in: header
    name: Rightmove-Agent-ID
    operations:
    - getCommercialPropertyDetails
    required: true
  api: Rightmove Commercial Listings API
  applied_to: all four operations carry a security requirement referencing this scheme
  credentials: ClientId + ClientKey issued by the Rightmove Data Feed Team, presented base64-encoded
  declared_in_spec:
    authorizationUrl: /oauth/token
    flows:
    - implicit
    scopes: {}
    type: oauth2
  defect: The published securityScheme declares an `implicit` flow with an authorizationUrl of /oauth/token and an empty scopes map, which contradicts the prose and the authentication page — both document the client_credentials grant with a token endpoint. There is also no top-level `security` in the document. Recorded as served; the correction is captured in overlays/rightmove-commercial-listings-overlay.yaml rather than by editing the harvested spec.
  documented_flow: clientCredentials
  name: OAuth2
  request_header: 'Authorization: Bearer <ACCESS_TOKEN>'
  scopes_implemented: false
  scopes_note: Scopes "are not currently required or implemented" per the portal authentication page.
  sources:
  - openapi/rightmove-commercial-listings-openapi.yml
  - https://api-docs.rightmove.co.uk/authentication
  token_url: /oauth/token
  token_url_examples:
  - https://api-services.rightmove.co.uk/oauth/token
  - https://api-services.adftest.rightmove.com/oauth/token
  type: oauth2
- anonymous_reachability:
    note: every path on adfapi.rightmove.co.uk refuses anonymous callers
    probed: '2026-07-26'
    status: 403
  api: Rightmove Real Time Data Feed API
  certificate_providers: Only certificate providers on Rightmove's supported list may be used; the list is obtained from the Data Feed Team.
  delivery: keystore emailed; password sent separately by SMS to a supplied mobile number
  documented_in: RTDF API Web Services Specification v1.4.1, section 2 "Authentication and Security"
  ip_allowlisting: Not recommended — Rightmove's outbound IPs can change without notice. Allowlist the user-agent instead, or request the current IPs from the Data Feed Team.
  mechanism: Rightmove issues a keystore containing a private key and an X.509 client certificate. Format is chosen by the integrator — JKS or JCEKS for Java, PKCS#12 for Windows applications, PEM for other languages.
  name: MutualTLS
  outbound_user_agent: rightmove-datafeed/1.0
  request_identifiers:
  - Network_ID
  - Branch_ID
  - Agent_Ref
  sources:
  - https://media.rightmove.co.uk/ps/pdf/guides/adf/Rightmove_Real_Time_Datafeed_Specification.pdf
  tls:
    documented_minimum: TLS 1.1 or 1.2 (section 2.1.1); TLS 1.0 and 1.1 support was removed in spec v1.3.6, so treat 1.2 as the floor.
    media_servers: integrator media servers must support TLS 1.2 or Rightmove cannot download images
    ssl: not supported
  type: mutualTLS
slug: rightmove-authentication
source_filename: rightmove-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-26'\nmethod: searched\nsource: openapi/rightmove-commercial-listings-openapi.yml\ndocs:\n- https://api-docs.rightmove.co.uk/authentication\n- https://api-docs.rightmove.co.uk/docs/property-feed-api-product/1/overview\n- https://media.rightmove.co.uk/ps/pdf/guides/adf/Rightmove_Real_Time_Datafeed_Specification.pdf\nsummary:\n  types: [oauth2, mutualTLS]\n  oauth2_flows: [clientCredentials]\n  api_key_in: []\n  gate: >-\n    Every credential for every environment — test and production, both APIs — is\n    issued case by case by the Rightmove Data Feed Team. Nothing is self-serve.\nschemes:\n- name: OAuth2\n  api: Rightmove Commercial Listings API\n  type: oauth2\n  documented_flow: clientCredentials\n  token_url: /oauth/token\n  token_url_examples:\n  - https://api-services.rightmove.co.uk/oauth/token\n  - https://api-services.adftest.rightmove.com/oauth/token\n  credentials: ClientId + ClientKey issued by the Rightmove Data Feed Team, presented base64-encoded\n\
  \  request_header: 'Authorization: Bearer <ACCESS_TOKEN>'\n  scopes_implemented: false\n  scopes_note: Scopes \"are not currently required or implemented\" per the portal authentication page.\n  applied_to: all four operations carry a security requirement referencing this scheme\n  declared_in_spec:\n    type: oauth2\n    flows: [implicit]\n    authorizationUrl: /oauth/token\n    scopes: {}\n  defect: >-\n    The published securityScheme declares an `implicit` flow with an\n    authorizationUrl of /oauth/token and an empty scopes map, which contradicts\n    the prose and the authentication page — both document the client_credentials\n    grant with a token endpoint. There is also no top-level `security` in the\n    document. Recorded as served; the correction is captured in\n    overlays/rightmove-commercial-listings-overlay.yaml rather than by editing the\n    harvested spec.\n  additional_headers:\n  - name: Rightmove-Agent-ID\n    in: header\n    required: true\n    operations: [getCommercialPropertyDetails]\n\
  \  sources:\n  - openapi/rightmove-commercial-listings-openapi.yml\n  - https://api-docs.rightmove.co.uk/authentication\n- name: MutualTLS\n  api: Rightmove Real Time Data Feed API\n  type: mutualTLS\n  documented_in: RTDF API Web Services Specification v1.4.1, section 2 \"Authentication and Security\"\n  mechanism: >-\n    Rightmove issues a keystore containing a private key and an X.509 client\n    certificate. Format is chosen by the integrator — JKS or JCEKS for Java,\n    PKCS#12 for Windows applications, PEM for other languages.\n  delivery: keystore emailed; password sent separately by SMS to a supplied mobile number\n  certificate_providers: >-\n    Only certificate providers on Rightmove's supported list may be used; the list\n    is obtained from the Data Feed Team.\n  tls:\n    documented_minimum: >-\n      TLS 1.1 or 1.2 (section 2.1.1); TLS 1.0 and 1.1 support was removed in spec\n      v1.3.6, so treat 1.2 as the floor.\n    ssl: not supported\n    media_servers: integrator\
  \ media servers must support TLS 1.2 or Rightmove cannot download images\n  request_identifiers: [Network_ID, Branch_ID, Agent_Ref]\n  outbound_user_agent: rightmove-datafeed/1.0\n  ip_allowlisting: >-\n    Not recommended — Rightmove's outbound IPs can change without notice.\n    Allowlist the user-agent instead, or request the current IPs from the Data\n    Feed Team.\n  anonymous_reachability:\n    probed: '2026-07-26'\n    status: 403\n    note: every path on adfapi.rightmove.co.uk refuses anonymous callers\n  sources:\n  - https://media.rightmove.co.uk/ps/pdf/guides/adf/Rightmove_Real_Time_Datafeed_Specification.pdf\nopenid_connect:\n  supported: false\n  evidence: No /.well-known/openid-configuration on any host (see well-known/rightmove-well-known.yml).\nonboarding:\n  contact: adfsupport@rightmove.co.uk\n  classification: application-approval\n  requirements:\n  - Accept the RTDF End User Licence Agreement with Rightmove Group Limited.\n  - Submit the ADF Provider Contact Form.\n\
  \  - Complete a supervised testing cycle before live credentials are released.\n  - 'In practice: act for a Rightmove member agent — RTDF calls require a Rightmove-issued Network_ID and Branch_ID.'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rightmove/refs/heads/main/authentication/rightmove-authentication.yml
summary_line: oauth2/mutualTLS · 2 schemes
tags:
- Real-Estate
- United Kingdom
- Property Listings
- Property Portal
- PropTech
- Rentals
- Commercial Real Estate
- Data Feed
---
