---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: probed
name: Purplelab Authentication
name_suffix: Authentication
oauth_flows: []
overview: PurpleLab declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: PurpleLab
provider_slug: purplelab
scheme_count: 0
schemes: []
slug: purplelab-authentication
source_filename: purplelab-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: probed\nsource: >-\n  Anonymous HTTPS probes of https://portal.purplelab.com/, https://www.healthnexus.io/,\n  https://api.healthnexus.io/ and https://api.purplelab.com/, plus\n  https://healthnexus-sso.purplelab.com/login?domain=portal.purplelab.com, 2026-08-26.\nnote: >-\n  POINTER DELIBERATELY WITHHELD. This artifact is written from live probes, not from provider\n  documentation - PurpleLab publishes NO authentication documentation of any kind. The scorer's\n  `authentication_documented` check credits a provider for documenting authentication, so NO\n  `Authentication` pointer is emitted in apis.yml. A later run should not \"fix\" that omission unless\n  PurpleLab actually publishes an auth page. What follows is our measurement of the deployed auth\n  architecture, and it is labelled as such throughout.\n\ndocumented_by_provider: false\ndocs_url: null\n\nsecurity_schemes: []\nsecurity_schemes_note: >-\n  Cannot be enumerated. No OpenAPI\
  \ exists to read securitySchemes from, and no OAuth/OIDC discovery\n  document is served anonymously on any host.\n\nobserved_architecture:\n  summary: >-\n    HealthNexus is protected by a bespoke first-party SSO service fronted by an AWS API Gateway. The\n    browser flow is: an unauthenticated request to the customer portal is 307-redirected to a\n    checklogin endpoint on the API gateway, which in turn 302-redirects to a React SSO application\n    on a purplelab.com subdomain.\n  flow:\n  - step: 1\n    request: GET https://portal.purplelab.com/\n    http_status: 307\n    location: >-\n      https://api.healthnexus.io/healthnexussso/checklogin?returnUrl=https%3A%2F%2Fportal.purplelab.com%2F\n    finding: >-\n      The customer portal delegates all authentication to api.healthnexus.io. This redirect is also\n      what established healthnexus.io as a PurpleLab-controlled domain.\n  - step: 2\n    request: GET https://api.healthnexus.io/healthnexussso/checklogin\n    http_status: 302\n\
  \    location: https://healthnexus-sso.purplelab.com/setup/...\n    finding: >-\n      The gateway hands off to the SSO application. This is the only api.healthnexus.io path found\n      that does NOT return 403 to an anonymous caller.\n  - step: 3\n    request: GET https://healthnexus-sso.purplelab.com/login?domain=portal.purplelab.com\n    http_status: 200\n    content_type: text/html\n    finding: >-\n      A 1,766-byte React single-page application, <meta name=\"description\" content=\"HealthNexus SSO\">.\n      The login UI and any identity-provider configuration are rendered client-side, so no\n      server-side auth metadata is readable.\n  - step: 4\n    request: GET https://www.healthnexus.io/\n    http_status: 307\n    location: https://api.healthnexus.io/healthnexussso/checklogin?returnUrl=...\n    finding: The whole healthnexus.io application is gated by the same flow.\n\napi_host_posture:\n- host: api.healthnexus.io\n  gateway: AWS API Gateway\n  anonymous_response:\n    http_status:\
  \ 403\n    content_type: application/json\n    body: '{\"message\":\"Forbidden\"}'\n  finding: >-\n    Every anonymous path returns 403, including /.well-known/* and every spec path probed. This is\n    the API Gateway default for a missing or invalid authorization header on a known route, and for\n    unknown routes. It is a closed door, not a documented scheme.\n- host: api.purplelab.com\n  gateway: unidentified (WSGI/Flask-style error envelope)\n  anonymous_response:\n    http_status: 200\n    content_type: application/json\n    body: '{}'\n  finding: >-\n    The root answers 200 with an empty JSON object; unknown paths return a bespoke JSON 404 envelope\n    ({\"error\": \"404 Not Found: The requested URL was not found on the server...\"}). No\n    WWW-Authenticate challenge is issued, so the auth scheme for this host could not be observed\n    without knowing a real route - and routes are not published.\n\noauth:\n  discovery_document: false\n  authorization_server_metadata:\n   \
  \ url: https://api.healthnexus.io/.well-known/oauth-authorization-server\n    http_status: 403\n  protected_resource_metadata:\n    url: https://api.healthnexus.io/.well-known/oauth-protected-resource\n    http_status: 403\n  openid_configuration:\n    url: https://api.purplelab.com/.well-known/openid-configuration\n    http_status: 404\n  conclusion: >-\n    Undetermined. The SSO service name (healthnexussso) and the redirect chain are consistent with\n    either a bespoke session scheme or an OAuth/OIDC implementation without published metadata.\n    Recorded as unknown rather than guessed - see conformance/purplelab-conformance.yml#oauth2.\n\napi_key_scheme:\n  documented: false\n  prefix: null\n  finding: No API-key format, header name, or issuance process is published.\n\nscopes:\n  present: unknown\n  artifact: null\n  finding: >-\n    No scopes/ artifact is written. scopes/ is OAuth-only per the pipeline contract, and no OAuth\n    surface could be confirmed, so an empty scopes\
  \ file would assert more than was measured.\n\nagent_impact: >-\n  There is no credential an agent can obtain, and no document telling it what to send. Every\n  authenticated surface requires a browser-driven SSO session established after an enterprise\n  contract.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/purplelab/refs/heads/main/authentication/purplelab-authentication.yml
summary_line: 0 schemes
tags:
- Healthcare
- Health Data
- Real-World Data
- Real-World Evidence
- Medical Claims
- Pharmacy Claims
- Provider Data
- Healthcare Analytics
- Life Sciences
- Data Products
- HIPAA
- Company
---
