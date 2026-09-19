---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 4
method: searched
name: Proofpoint Authentication
name_suffix: Authentication
oauth_flows: []
overview: Proofpoint declares 5 security scheme(s) across its OpenAPI definitions.
provider_name: Proofpoint
provider_slug: proofpoint
scheme_count: 5
schemes:
- anonymous_allowed:
    endpoint: /v2/url/decode
    note: The URL Decoder documentation says credentials MAY be used — the endpoint is documented with and without --user, making it the one anonymously callable Proofpoint API operation. Unauthenticated calls are throttled on a shared pool.
  applies_to:
  - proofpoint-tap
  - proofpoint-essentials-siem
  credential: HTTP Basic with a "service principal" as the username and a "secret" as the password. Both are minted by an administrator on the TAP (or Essentials) Settings page; there is no self-service developer signup.
  docs: https://help.proofpoint.com/Threat_Insight_Dashboard/API_Documentation/SIEM_API
  id: tap-basic
  methods_allowed: GET for every endpoint except /v2/url/decode, which is POST
  scheme: basic
  transport: TLS required ("Each request MUST use SSL")
  type: http
- applies_to:
  - proofpoint-threat-protection-reports
  credential: API key and secret generated in the Threat Protection admin console ("generate a new API key and secret for the Threat Protection API").
  discovery:
    note: auth.proofpoint.com publishes no authorization-server metadata; the token endpoint is known only from the prose in the Reports API documentation.
    oauth_authorization_server: 404
    openid_configuration: 404
  docs: https://help.proofpoint.com/Threat_Insight_Dashboard/API_Documentation/Reports_API
  expires_in: 3600
  flow: clientCredentials
  header: 'Authorization: Bearer <token>'
  id: threatprotection-oauth2
  scopes: []
  scopes_note: No scopes are documented. The token response carries only access_token, token_type and expires_in, so there is no published permission surface to model — which is why no scopes/ artifact was written.
  token_endpoint: https://auth.proofpoint.com/v1/token
  token_type: Bearer
  type: oauth2
- applies_to:
  - proofpoint-et-intelligence
  credential: 'A single opaque API key, sent raw in the Authorization header with no scheme prefix: "Authorization: SECRETKEY". Keys are issued at https://etadmin.proofpoint.com/api-access to customers who have paid for API access.'
  docs: https://apidocs.emergingthreats.net/
  id: et-api-key
  in: header
  name: Authorization
  type: apiKey
- applies_to:
  - proofpoint-psat-results
  credential: A regional API key passed to the Results API. The first-party Python client is constructed as PSATClient(Region.US, "<api_key>"), and the published apiDoc description carries a dedicated Authentication entry.
  docs: https://proofpoint.securityeducation.com/api/reporting/documentation/
  id: psat-api-key
  type: apiKey
- applies_to:
  - proofpoint-secure-email-relay
  credential: Secure Email Relay separates a Configuration Token from an Email Submission Token; the api-docs.ser.proofpoint.com navigation exposes both as distinct authentication routes. The documentation renders client-side and the token endpoints could not be read without executing the app, so the exact endpoints are recorded as unread rather than guessed.
  docs: https://api-docs.ser.proofpoint.com/authentication/email-submission-token
  flow: clientCredentials
  id: ser-oauth
  type: oauth2
slug: proofpoint-authentication
source_filename: proofpoint-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-13'\nmethod: searched\nsource: 'Proofpoint public API documentation: help.proofpoint.com/Threat_Insight_Dashboard/API_Documentation/*,\n  help.proofpoint.com/Essentials/Additional_Resources/API_Documentation/Essentials_Threat_API,\n  apidocs.emergingthreats.net, proofpoint.securityeducation.com/api/reporting/documentation/'\nnote: 'Derived from documentation, not from a specification — Proofpoint publishes no\n  OpenAPI securitySchemes anywhere. Three distinct and non-interchangeable auth models\n  are in production across the estate; a client written for one will not work against\n  another.'\nsummary:\n  schemes_count: 3\n  oauth2: true\n  oidc: false\n  mtls: false\n  scopes_documented: false\nschemes:\n- id: tap-basic\n  type: http\n  scheme: basic\n  applies_to:\n  - proofpoint-tap\n  - proofpoint-essentials-siem\n  credential: 'HTTP Basic with a \"service principal\" as the username and a \"secret\" as\n    the password. Both are minted by an administrator\
  \ on the TAP (or Essentials)\n    Settings page; there is no self-service developer signup.'\n  transport: TLS required (\"Each request MUST use SSL\")\n  methods_allowed: GET for every endpoint except /v2/url/decode, which is POST\n  anonymous_allowed:\n    endpoint: /v2/url/decode\n    note: 'The URL Decoder documentation says credentials MAY be used — the endpoint is\n      documented with and without --user, making it the one anonymously callable\n      Proofpoint API operation. Unauthenticated calls are throttled on a shared pool.'\n  docs: https://help.proofpoint.com/Threat_Insight_Dashboard/API_Documentation/SIEM_API\n- id: threatprotection-oauth2\n  type: oauth2\n  flow: clientCredentials\n  applies_to:\n  - proofpoint-threat-protection-reports\n  token_endpoint: https://auth.proofpoint.com/v1/token\n  token_type: Bearer\n  expires_in: 3600\n  header: 'Authorization: Bearer <token>'\n  credential: API key and secret generated in the Threat Protection admin console\n    (\"generate\
  \ a new API key and secret for the Threat Protection API\").\n  scopes: []\n  scopes_note: 'No scopes are documented. The token response carries only access_token,\n    token_type and expires_in, so there is no published permission surface to model —\n    which is why no scopes/ artifact was written.'\n  discovery:\n    oauth_authorization_server: 404\n    openid_configuration: 404\n    note: auth.proofpoint.com publishes no authorization-server metadata; the token\n      endpoint is known only from the prose in the Reports API documentation.\n  docs: https://help.proofpoint.com/Threat_Insight_Dashboard/API_Documentation/Reports_API\n- id: et-api-key\n  type: apiKey\n  in: header\n  name: Authorization\n  applies_to:\n  - proofpoint-et-intelligence\n  credential: 'A single opaque API key, sent raw in the Authorization header with no\n    scheme prefix: \"Authorization: SECRETKEY\". Keys are issued at\n    https://etadmin.proofpoint.com/api-access to customers who have paid for API access.'\n\
  \  docs: https://apidocs.emergingthreats.net/\n- id: psat-api-key\n  type: apiKey\n  applies_to:\n  - proofpoint-psat-results\n  credential: 'A regional API key passed to the Results API. The first-party Python\n    client is constructed as PSATClient(Region.US, \"<api_key>\"), and the published\n    apiDoc description carries a dedicated Authentication entry.'\n  docs: https://proofpoint.securityeducation.com/api/reporting/documentation/\n- id: ser-oauth\n  type: oauth2\n  flow: clientCredentials\n  applies_to:\n  - proofpoint-secure-email-relay\n  credential: 'Secure Email Relay separates a Configuration Token from an Email\n    Submission Token; the api-docs.ser.proofpoint.com navigation exposes both as\n    distinct authentication routes. The documentation renders client-side and the token\n    endpoints could not be read without executing the app, so the exact endpoints are\n    recorded as unread rather than guessed.'\n  docs: https://api-docs.ser.proofpoint.com/authentication/email-submission-token\n\
  gaps:\n- 'No self-service credential issuance on any surface: every key is minted by an\n  administrator inside a paid tenant, so an agent or developer cannot obtain access\n  without an existing Proofpoint contract.'\n- No OAuth scope reference is published for either OAuth surface.\n- No authorization-server metadata document is served on auth.proofpoint.com.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/proofpoint/refs/heads/main/authentication/proofpoint-authentication.yml
summary_line: 5 schemes
tags:
- Security
- Cybersecurity
- Email Security
- Threat Intelligence
- Data Loss Prevention
- Security Awareness Training
- Insider Threat
- SIEM
- Compliance
- Email
---
