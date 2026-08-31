---
api_key_in: []
auth_types: []
description: Tridge publishes no API authentication documentation. What is recorded here was observed by probe, not read from a developer reference, and it describes the PLATFORM sign-in used by the Tridge web application — it is not confirmed to be the credential model for the commercial data API, which is arranged through sales.
kind: authentication
layout: security
method: probed
name: Tridge Authentication
name_suffix: Authentication
oauth_flows: []
overview: Tridge declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Tridge
provider_slug: tridge
scheme_count: 1
schemes:
- authorization_url: https://accounts.tridge.com/oauth/authorize
  evidence:
  - note: 'Location: https://accounts.tridge.com/oauth/authorize?response_type=code&client_id=<uuid>&state=…&redirect_uri=https%3A%2F%2Fwww.tridge.com%2Flogin%2Fclient&hl=en — an RFC 6749 authorization-code request issued by Tridge''s own first-party web client.'
    status: 302
    url: https://www.tridge.com/login
  - note: Authorization endpoint responds to an anonymous request with a redirect.
    status: 302
    url: https://accounts.tridge.com/oauth/authorize
  - note: Token endpoint exists and rejects GET with 405 Method Not Allowed, consistent with a POST-only OAuth token endpoint.
    status: 405
    url: https://accounts.tridge.com/oauth/token
  flow: authorizationCode
  id: platform_oauth2_authorization_code
  note: 'No scope values could be established: no scope parameter appears in the observed authorization request and no scopes/permissions reference page is published, so scopes/tridge-scopes.yml is deliberately not written rather than filled with guesses.'
  observed: true
  scopes_documented: false
  token_url: https://accounts.tridge.com/oauth/token
  type: oauth2
slug: tridge-authentication
source_filename: tridge-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-30'\nmethod: probed\nsource: 'Observed redirect chain from https://www.tridge.com/login (HTTP 302) to\n  https://accounts.tridge.com/oauth/authorize, plus direct probes of accounts.tridge.com\n  and api.tridge.com.'\nname: Tridge authentication\ndescription: 'Tridge publishes no API authentication documentation. What is recorded\n  here was observed by probe, not read from a developer reference, and it describes\n  the PLATFORM sign-in used by the Tridge web application — it is not confirmed to be\n  the credential model for the commercial data API, which is arranged through sales.'\ndocumented: false\ndocs: null\nschemes:\n- id: platform_oauth2_authorization_code\n  type: oauth2\n  flow: authorizationCode\n  observed: true\n  authorization_url: https://accounts.tridge.com/oauth/authorize\n  token_url: https://accounts.tridge.com/oauth/token\n  evidence:\n  - url: https://www.tridge.com/login\n    status: 302\n    note: 'Location: https://accounts.tridge.com/oauth/authorize?response_type=code&client_id=<uuid>&state=…&redirect_uri=https%3A%2F%2Fwww.tridge.com%2Flogin%2Fclient&hl=en\n\
  \      — an RFC 6749 authorization-code request issued by Tridge''s own first-party\n      web client.'\n  - url: https://accounts.tridge.com/oauth/authorize\n    status: 302\n    note: Authorization endpoint responds to an anonymous request with a redirect.\n  - url: https://accounts.tridge.com/oauth/token\n    status: 405\n    note: 'Token endpoint exists and rejects GET with 405 Method Not Allowed, consistent\n      with a POST-only OAuth token endpoint.'\n  scopes_documented: false\n  note: 'No scope values could be established: no scope parameter appears in the\n    observed authorization request and no scopes/permissions reference page is\n    published, so scopes/tridge-scopes.yml is deliberately not written rather than\n    filled with guesses.'\ndiscovery:\n  openid_configuration: null\n  oauth_authorization_server: null\n  note: 'Neither RFC 8414 (/.well-known/oauth-authorization-server) nor OpenID Connect\n    discovery (/.well-known/openid-configuration) is served on accounts.tridge.com;\n\
  \    both return 404. An OAuth client cannot bootstrap from metadata and must be\n    configured out of band.'\napi_surface:\n- host: api.tridge.com\n  path: /graphql\n  status: 403\n  body: crc rejected\n  note: 'Anonymous GET and POST are rejected by an origin/CSRF gate (\"crc rejected\",\n    served by gunicorn) before any authentication challenge is issued — no\n    WWW-Authenticate header and no OAuth challenge is returned, so the credential\n    type for this surface could not be determined anonymously. www.tridge.com/robots.txt\n    additionally disallows /graphql and /api/ for all user agents.'\ngaps:\n- No public API authentication documentation.\n- No API key issuance, key-prefix convention, or self-serve credential flow published.\n- No scope or permission model published.\n- No authorization-server metadata document, so no machine-readable auth discovery.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tridge/refs/heads/main/authentication/tridge-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Agriculture
- Food
- Trade
- Commodities
- Market Data
- Supply Chain
- Sourcing
- Analytics
- Price Data
- Intelligence
- Artificial Intelligence
---
