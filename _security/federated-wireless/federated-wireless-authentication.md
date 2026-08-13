---
api_key_in: []
auth_types:
- oauth2
description: 'Federated Wireless publishes no OpenAPI or Swagger document on any host, so this profile could not be derived from securitySchemes. It was assembled entirely from live probes. There is exactly one publicly documented authentication mechanism — the OAuth 2.1 authorization server that fronts the MCP server on federatedwireless.ai. Every other Federated Wireless API surface is authenticated but undocumented: the three Spectrum Controller AWS API Gateway endpoints return 403 MissingAuthenticationTokenException to anonymous callers without advertising a scheme, and the regulated SAS-CBSD and 6 GHz AFC interfaces are not reachable from the public internet at all.'
kind: authentication
layout: security
method: probed
name: Federated Wireless Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Federated Wireless secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Federated Wireless
provider_slug: federated-wireless
scheme_count: 1
schemes:
- applies_to: https://federatedwireless.ai/wp-json/mcp/mcp-oauth-server
  bearer_methods:
  - header
  detail: scopes/federated-wireless-scopes.yml
  flows:
  - authorizationUrl: https://federatedwireless.ai/oauth/authorize
    flow: authorizationCode
    pkce: required (S256)
    public_client: true
    revocationUrl: https://federatedwireless.ai/oauth/revoke
    scopes:
    - mcp
    tokenUrl: https://federatedwireless.ai/oauth/token
  issuer: https://federatedwireless.ai
  name: FederatedWirelessMCPOAuth
  source: https://federatedwireless.ai/.well-known/oauth-authorization-server
  type: oauth2
slug: federated-wireless-authentication
source_filename: federated-wireless-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: probed\nsource: >-\n  https://federatedwireless.ai/.well-known/oauth-authorization-server +\n  https://federatedwireless.ai/.well-known/oauth-protected-resource + live probes of every Federated\n  Wireless API host\ndocs: null\ndescription: >-\n  Federated Wireless publishes no OpenAPI or Swagger document on any host, so this profile could not\n  be derived from securitySchemes. It was assembled entirely from live probes. There is exactly one\n  publicly documented authentication mechanism — the OAuth 2.1 authorization server that fronts the\n  MCP server on federatedwireless.ai. Every other Federated Wireless API surface is authenticated but\n  undocumented: the three Spectrum Controller AWS API Gateway endpoints return 403\n  MissingAuthenticationTokenException to anonymous callers without advertising a scheme, and the\n  regulated SAS-CBSD and 6 GHz AFC interfaces are not reachable from the public internet at all.\nsummary:\n  types: [oauth2]\n\
  \  api_key_in: []\n  oauth2_flows: [authorizationCode]\n  documented_publicly: false\n  note: >-\n    `types` lists only what is observable. It is a floor, not a complete picture — the product APIs\n    certainly authenticate, but Federated Wireless publishes nothing that says how.\nschemes:\n- name: FederatedWirelessMCPOAuth\n  type: oauth2\n  source: https://federatedwireless.ai/.well-known/oauth-authorization-server\n  applies_to: https://federatedwireless.ai/wp-json/mcp/mcp-oauth-server\n  issuer: https://federatedwireless.ai\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://federatedwireless.ai/oauth/authorize\n    tokenUrl: https://federatedwireless.ai/oauth/token\n    revocationUrl: https://federatedwireless.ai/oauth/revoke\n    scopes: [mcp]\n    pkce: required (S256)\n    public_client: true\n  bearer_methods: [header]\n  detail: scopes/federated-wireless-scopes.yml\nundocumented_surfaces:\n- surface: Spectrum Controller external SAS API\n  base_url: https://spectrum-api.federatedwireless.com/v1\n\
  \  observed: >-\n    HTTP 403 {\"message\": \"Missing Authentication Token\"}; x-amzn-errortype\n    MissingAuthenticationTokenException. AWS API Gateway\n    (d-d3psb9cl3e.execute-api.us-west-2.amazonaws.com). No WWW-Authenticate header, so the scheme\n    (IAM SigV4, Cognito authorizer, API key or custom Lambda authorizer) is not observable anonymously.\n- surface: Spectrum IAM API\n  base_url: https://spectrum-iam.federatedwireless.com/v1\n  observed: HTTP 403 MissingAuthenticationTokenException. AWS API Gateway behind CloudFront.\n  note: >-\n    The name and the fact that the Spectrum Controller web app calls it as IAM_BASE_URL indicate this\n    is the identity/session service for the customer portal, but no scheme is published.\n- surface: Spectrum KPI / analytics + reporting API\n  base_url: https://spectrum-kpi.federatedwireless.com/v2.0\n  observed: HTTP 403 MissingAuthenticationTokenException. AWS API Gateway behind CloudFront.\n- surface: SAS-CBSD interface\n  base_url: https://sas.federatedwireless.com\n\
  \  observed: TCP 443 refused from the public internet; DNS resolves to 35.166.171.66 (AWS us-west-2).\n  expected_scheme: >-\n    Mutual TLS with CBSD client certificates, per WInnForum WINNF-TS-0016 (SAS to CBSD Technical\n    Specification) and FCC Part 96. Recorded as the regulated protocol's requirement, NOT as an\n    observation — no handshake was completed.\n- surface: 6 GHz AFC device interface\n  base_url: https://afc.federatedwireless.com\n  observed: >-\n    TCP 443 refused from the public internet; DNS resolves to an AWS ELB\n    (a98859f24fc724909b8a256a877bbb50-431290955.us-west-2.elb.amazonaws.com).\n  expected_scheme: >-\n    Certified-device / proxy authentication per the WInnForum AFC System to AFC Device interface.\n    Recorded as the protocol's requirement, not as an observation.\n- surface: MyFederated customer portal\n  base_url: https://myfederated.federatedwireless.com\n  observed: >-\n    Zendesk-hosted (federatedwirelessinc.zendesk.com). /hc/en-us returns 403\
  \ to an anonymous visitor;\n    only the Help Center REST API is open, and it exposes six FAQ articles about course access and\n    password resets. Sign-in required for everything else.\nx-evidence:\n  fetched: '2026-08-12'\n  probes:\n  - url: https://federatedwireless.ai/.well-known/oauth-authorization-server\n    status: 200\n  - url: https://federatedwireless.ai/wp-json/mcp/mcp-oauth-server\n    status: 401\n  - url: https://spectrum-api.federatedwireless.com/v1\n    status: 403\n  - url: https://spectrum-iam.federatedwireless.com/v1\n    status: 403\n  - url: https://spectrum-kpi.federatedwireless.com/v1\n    status: 403\n  - url: https://myfederated.federatedwireless.com/hc/en-us\n    status: 403\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/federated-wireless/refs/heads/main/authentication/federated-wireless-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Company
- Spectrum
- CBRS
- Wireless
- Telecommunications
- Private 5G
- Shared Spectrum
- Spectrum Access System
- 6 GHz
- Network Planning
- RF Engineering
- Government
---
