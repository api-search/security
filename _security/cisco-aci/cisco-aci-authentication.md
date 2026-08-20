---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: searched
name: Cisco Aci Authentication
name_suffix: Authentication
oauth_flows: []
overview: Cisco ACI declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: Cisco ACI
provider_slug: cisco-aci
scheme_count: 3
schemes:
- description: Username/password authentication against a special subset of request URIs — aaaLogin, aaaLogout and aaaRefresh — used as the DN targets of a POST. The payload carries an aaaUser managed object with name and pwd attributes. The response returns an authentication token both as a Set-Cookie header and as the token attribute of the aaaLogin object (XPath /imdata/aaaLogin/@token). Subsequent requests present that value as a cookie named APIC-cookie.
  id: aaa-login-session-cookie
  in: cookie
  login:
    encodings:
    - json
    - xml
    method: POST
    path: /api/aaaLogin.json
    request_body: '{"aaaUser": {"attributes": {"name": "<username>", "pwd": "<password>"}}}'
  logout:
    method: POST
    path: /api/aaaLogout.json
  name: APIC-cookie
  primary: true
  refresh:
    description: The session must be refreshed within the timeout window or the token expires. The token changes on every refresh.
    method: POST or GET
    path: /api/aaaRefresh.json
  session:
    default_timeout_note: '"The default session timeout period is 600 seconds or 10 minutes." The aaaLogin response returns the actual value in refreshTimeoutSeconds; the guide''s worked example shows 300.'
    default_timeout_seconds: 600
    expiry_behavior: An expired session returns HTTP 403. The CiscoDevNet ACI MCP server treats 403 as the signal to re-run aaaLogin transparently.
    timeout_attribute: refreshTimeoutSeconds
  type: session-cookie
- alternate_in: query
  alternate_name: challenge
  description: An optional additional token, requested by adding ?gui-token-request=yes to the aaaLogin call. The response body then carries a "urlToken" attribute whose value must accompany every subsequent request in this session, either as an APIC-challenge HTTP header or as a challenge= URI parameter. Applies to REST API calls; not available to the browser.
  id: gui-challenge-token
  in: header
  name: APIC-challenge
  primary: false
  type: challenge-token
- description: The APIC supports authentication realms beyond the local user store. GET /api/aaaListDomains.json returns the valid login domains for a controller (the guide's example returns "ExampleRadius" and "local"), and the login name is prefixed with the domain to authenticate against RADIUS/TACACS+/LDAP.
  discovery:
    anonymous: true
    method: GET
    path: /api/aaaListDomains.json
  id: login-domains
  primary: false
  type: external-identity
slug: cisco-aci-authentication
source_filename: cisco-aci-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-19'\nmethod: searched\nsource: https://www.cisco.com/c/en/us/td/docs/dcn/aci/apic/all/apic-rest-api-configuration-guide/cisco-apic-rest-api-configuration-guide-42x-and-later/m_using_the_rest_api.html\ndocs: https://www.cisco.com/c/en/us/td/docs/dcn/aci/apic/all/apic-rest-api-configuration-guide/cisco-apic-rest-api-configuration-guide-42x-and-later/m_using_the_rest_api.html\nnote: >-\n  Derived from the published Cisco APIC REST API Configuration Guide (Release 4.2(x) and Later), chapter\n  \"Using the REST API\", read 2026-08-19. There is no OpenAPI securitySchemes block to derive from — Cisco\n  publishes no machine-readable contract for this API — so every field below is quoted from the human\n  documentation and cross-checked against the reference implementation in the CiscoDevNet ACI MCP server.\napi: Cisco APIC REST API\ntransport: >-\n  HTTPS only by default. The guide states: \"For security, only HTTPS is enabled as the default mode for API\n  communications.\
  \ HTTP and HTTP-to-HTTPS redirection can be enabled if desired, but are less secure.\"\nschemes:\n- id: aaa-login-session-cookie\n  type: session-cookie\n  primary: true\n  name: APIC-cookie\n  in: cookie\n  description: >-\n    Username/password authentication against a special subset of request URIs — aaaLogin, aaaLogout and\n    aaaRefresh — used as the DN targets of a POST. The payload carries an aaaUser managed object with name\n    and pwd attributes. The response returns an authentication token both as a Set-Cookie header and as the\n    token attribute of the aaaLogin object (XPath /imdata/aaaLogin/@token). Subsequent requests present that\n    value as a cookie named APIC-cookie.\n  login:\n    method: POST\n    path: /api/aaaLogin.json\n    request_body: '{\"aaaUser\": {\"attributes\": {\"name\": \"<username>\", \"pwd\": \"<password>\"}}}'\n    encodings:\n    - json\n    - xml\n  logout:\n    method: POST\n    path: /api/aaaLogout.json\n  refresh:\n    method: POST or GET\n\
  \    path: /api/aaaRefresh.json\n    description: >-\n      The session must be refreshed within the timeout window or the token expires. The token changes on\n      every refresh.\n  session:\n    timeout_attribute: refreshTimeoutSeconds\n    default_timeout_seconds: 600\n    default_timeout_note: >-\n      \"The default session timeout period is 600 seconds or 10 minutes.\" The aaaLogin response returns the\n      actual value in refreshTimeoutSeconds; the guide's worked example shows 300.\n    expiry_behavior: >-\n      An expired session returns HTTP 403. The CiscoDevNet ACI MCP server treats 403 as the signal to\n      re-run aaaLogin transparently.\n- id: gui-challenge-token\n  type: challenge-token\n  primary: false\n  name: APIC-challenge\n  in: header\n  alternate_in: query\n  alternate_name: challenge\n  description: >-\n    An optional additional token, requested by adding ?gui-token-request=yes to the aaaLogin call. The\n    response body then carries a \"urlToken\" attribute\
  \ whose value must accompany every subsequent request in\n    this session, either as an APIC-challenge HTTP header or as a challenge= URI parameter. Applies to REST\n    API calls; not available to the browser.\n- id: login-domains\n  type: external-identity\n  primary: false\n  description: >-\n    The APIC supports authentication realms beyond the local user store. GET /api/aaaListDomains.json\n    returns the valid login domains for a controller (the guide's example returns \"ExampleRadius\" and\n    \"local\"), and the login name is prefixed with the domain to authenticate against RADIUS/TACACS+/LDAP.\n  discovery:\n    method: GET\n    path: /api/aaaListDomains.json\n    anonymous: true\noauth2: false\noauth2_note: >-\n  The APIC REST API does not use OAuth 2.0 or OpenID Connect, and declares no scopes. Authorization is\n  handled by the APIC's own RBAC model — security domains, roles and read/write privileges attached to the\n  aaaUser — not by bearer-token scopes. No scopes/ artifact\
  \ was written; there is no scope surface to record.\napi_keys: false\nmtls:\n  supported: true\n  note: >-\n    The guide documents \"Configuring a Custom Certificate for Cisco ACI HTTPS Access\", and ACI additionally\n    supports X.509 certificate/signature-based API authentication for automation accounts. The certificate\n    is installed on the customer's own controller, so there is no public endpoint to probe.\ngaps:\n- No published OpenAPI securitySchemes block, so no machine-readable auth description exists.\n- >-\n  No OAuth/OIDC and no scoped tokens: an automation credential is a full APIC user, and least-privilege has\n  to be expressed through APIC RBAC roles rather than through the token itself.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cisco-aci/refs/heads/main/authentication/cisco-aci-authentication.yml
summary_line: 3 schemes
tags:
- SDN
- Data-Center
- Networking
- Fabric
- Automation
- Enterprise
- Network Automation
- Infrastructure
- Controller
- REST API
---
