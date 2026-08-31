---
api_key_in: []
api_specs:
- filename: ics_postman_apis.htm
  format: yaml
  label: Ivanti Connect Secure REST API
  slug: ivanti-connect-secure-rest-api
  spec_type: Postman
  url: https://help.ivanti.com/ps/help/en_US/ICS/22.x/apig/rest_api_soln_guide/ics_postman_apis.htm
auth_types: []
description: Authentication profile for the three Ivanti secure-access APIs profiled in this repo. Read from the provider's own published REST API Solutions Guide and the Ivanti Neurons for Zero Trust Access API guide. None of these APIs use OAuth 2.0 or OpenID Connect — the appliance APIs use HTTP Basic with a server-minted api_key, and the nZTA tenant API uses a session cookie obtained from the admin sign-in flow.
kind: authentication
layout: security
method: searched
name: Pulse Authentication
name_suffix: Authentication
oauth_flows: []
overview: Pulse declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: Pulse
provider_slug: pulse
scheme_count: 0
schemes: []
slug: pulse-authentication
source_filename: pulse-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "specification: API Commons Authentication\nspecificationVersion: '0.1'\nprovider: Pulse\nproviderId: pulse\ngenerated: '2026-08-29'\nmethod: searched\nsource: https://help.ivanti.com/ps/help/en_US/ICS/22.x/apig/rest_api_soln_guide/ovw.htm\ndescription: >-\n  Authentication profile for the three Ivanti secure-access APIs profiled in this repo.\n  Read from the provider's own published REST API Solutions Guide and the Ivanti Neurons\n  for Zero Trust Access API guide. None of these APIs use OAuth 2.0 or OpenID Connect —\n  the appliance APIs use HTTP Basic with a server-minted api_key, and the nZTA tenant API\n  uses a session cookie obtained from the admin sign-in flow.\ndocs:\n  - https://help.ivanti.com/ps/help/en_US/ICS/22.x/apig/rest_api_soln_guide/ovw.htm\n  - https://help.ivanti.com/ps/help/en_US/IPS/vNow/pcs-pps-rest-api/overview.htm\n  - https://docs.ivanti.com/ps/help/en_us/nsa/22x/nsa-zta/api/retrieving-the-authentication-dsid\ntransport_security:\n  tls_required:\
  \ true\n  note: >-\n    \"The entire communication is over TLS.\" — REST API Solutions Guide, Authentication for\n    REST APIs. Appliance certificates are customer-installed; the guide notes callers must\n    have the appliance server CA in the curl trust store.\napis:\n  - api: Ivanti Connect Secure REST API\n    aid: pulse:ivanti-connect-secure-rest-api\n    schemes:\n      - id: realm_auth\n        type: http\n        scheme: basic\n        preferred: true\n        flow: >-\n          POST /api/v1/realm_auth with an HTTP Basic Authorization header carrying the\n          administrator username/password and a JSON body naming the admin realm\n          ({\"realm\": \"adminrealm\"}). The response returns a JSON body containing an\n          api_key. Where the realm enforces secondary authentication the first response\n          returns a resume_id instead, which is posted back to the same endpoint to obtain\n          the api_key.\n        credential_in: Authorization header (Basic)\n\
  \        token_field: api_key\n        subsequent_use: >-\n          The api_key value is used as the Basic-auth USERNAME with an EMPTY password on\n          every subsequent request.\n        lifetime: >-\n          Valid until the session timeout configured on the Admin role mapped to the admin\n          realm. After expiry the caller re-issues POST /api/v1/realm_auth.\n        docs: https://help.ivanti.com/ps/help/en_US/ICS/22.x/apig/rest_api_soln_guide/ovw.htm\n      - id: auth\n        type: http\n        scheme: basic\n        preferred: false\n        deprecated: true\n        deprecation_note: >-\n          \"Ivanti recommends using api/v1/realm_auth instead of api/v1/auth as it will not\n          be supported from 22.7R2.1 release onwards.\" — REST API Solutions Guide.\n        flow: >-\n          GET /api/v1/auth with an HTTP Basic Authorization header of the administrator\n          username/password against the Administrators auth server. Returns {\"api_key\": \"...\"}.\n\
  \        docs: https://help.ivanti.com/ps/help/en_US/ICS/22.x/apig/rest_api_soln_guide/ovw.htm\n    authorization_gate:\n      description: >-\n        REST access is not on by default. The administrator account must have the \"Allow\n        access to REST APIs\" option enabled, either from Authentication > Auth. Servers >\n        Administrators > Update Administrator in the admin console, or by answering y to\n        \"Do you want to enable REST API access for this administrator (y/n)\" at the serial\n        console during provisioning or admin creation. The api_key is invalidated when the\n        administrator account or the Allow REST API setting is toggled.\n      docs: https://help.ivanti.com/ps/help/en_US/ICS/22.x/apig/rest_api_soln_guide/ovw.htm\n    scopes: []\n    scopes_note: >-\n      There is no scope or permission-string vocabulary on this API. Authorization is\n      carried entirely by the admin role and realm the authenticating administrator is\n      mapped to, so\
  \ the granularity lives in appliance configuration, not in the token.\n  - api: Ivanti Policy Secure REST API\n    aid: pulse:ivanti-policy-secure-rest-api\n    same_as: pulse:ivanti-connect-secure-rest-api\n    note: >-\n      Ivanti Policy Secure shares the ICS/IPS REST API Solutions Guide and the same\n      /api/v1/realm_auth and /api/v1/auth mechanisms; only the resource tree under\n      /api/v1/configuration/uac differs.\n    docs: https://help.ivanti.com/ps/help/en_US/IPS/vNow/pcs-pps-rest-api/overview.htm\n  - api: Ivanti Neurons for Zero Trust Access REST API\n    aid: pulse:ivanti-neurons-zero-trust-rest-api\n    schemes:\n      - id: dsid-cookie\n        type: apiKey\n        in: cookie\n        name: DSID\n        preferred: true\n        flow: >-\n          The Data Set Identification (DSID) cookie is required for all API use. It is\n          obtained by driving the tenant admin sign-in flow: GET <tenant>/login/admin to\n          pick up the DSSIGNIN cookie, then POST to\n\
  \          <tenant>/dana-na/auth/<DSSIGNIN>/login.cgi with username, password and\n          realm \"zta-admin-users\", following the \"continue the session\" form\n          (formdatastr + xsauth) where a prior session is open. The DSID cookie on the\n          resulting session is then sent on every API call.\n        alternate_flow: >-\n          The DSID value can also be read by hand from browser devtools (Network >\n          Cookies) while signed into the nZTA tenant admin UI.\n        usage: 'curl -v --cookie \"DSID=<value>\" <api request url>'\n        docs: https://docs.ivanti.com/ps/help/en_us/nsa/22x/nsa-zta/api/retrieving-the-authentication-dsid\n    scopes: []\n    scopes_note: >-\n      No OAuth scopes are published. Access is bounded by the tenant and the admin realm\n      the DSID session was minted against.\noauth2: false\nopenid_connect: false\nmutual_tls: false\napi_keys: true\nnotes:\n  - >-\n    Both mechanisms are administrator-session-derived, not client-credential-derived:\
  \ there\n    is no developer key you can mint from a portal, and no machine-to-machine grant. An\n    agent calling either API is acting as a named appliance or tenant administrator.\n  - >-\n    ICS/IPS support SAML, OIDC, RADIUS, TACACS+ and 802.1X as authentication protocols for\n    the END USERS the product secures. Those are product features, not authentication for\n    the management API itself, and are recorded in conformance/pulse-conformance.yml rather\n    than here.\nmaintainers:\n  - FN: Kin Lane\n    email: kin@apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pulse/refs/heads/main/authentication/pulse-authentication.yml
summary_line: 0 schemes
tags:
- Ivanti
- Network Security
- Secure Access
- SSL VPN
- VPN
- Zero Trust
- ZTNA
- Network Access Control
- Remote Access
- Identity and Access Management
- Security
- Pulse Secure
---
