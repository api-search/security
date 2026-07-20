---
api_key_in: []
auth_types:
- http
description: ''
kind: authentication
layout: security
method: probed
name: Amplify Authentication
name_suffix: Authentication
oauth_flows: []
overview: Amplify secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Amplify
provider_slug: amplify
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: 'Sending "Authorization: Bearer <token>" changes the failure mode from the generic gate to token validation, and the returned stack trace shows the token being handed to google-auth-library''s OAuth2Client.verifyIdTokenAsync / verifySignedJwtWithCertsAsync inside a User.Auth handler. The API therefore authenticates callers with Google-issued OpenID Connect ID tokens (Google Sign-In), verified server-side against Google''s public certificates.'
  evidence:
  - body_error: 'Wrong number of segments in token: test'
    request: 'GET / with header "Authorization: Bearer test"'
    stack_frames:
    - _OAuth2Client.verifySignedJwtWithCertsAsync
    - _OAuth2Client.verifyIdTokenAsync
    - User.Auth
    status: 401
  in: header
  name: BearerIdToken
  parameter: Authorization
  scheme: bearer
  sources:
  - probe:https://api.getamplifylife.com/
  type: http
slug: amplify-authentication
source_filename: amplify-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live HTTP probes of https://api.getamplifylife.com/ (2026-07-20)\ndocs: null\nsummary:\n  types:\n  - http\n  api_key_in: []\n  oauth2_flows: []\n  note: >-\n    Amplify publishes no authentication documentation. The profile below is derived\n    entirely from observed responses of the live, gated production API host. It is\n    an observation of behaviour, not a provider claim.\nschemes:\n- name: BearerIdToken\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  in: header\n  parameter: Authorization\n  sources:\n  - probe:https://api.getamplifylife.com/\n  description: >-\n    Sending \"Authorization: Bearer <token>\" changes the failure mode from the\n    generic gate to token validation, and the returned stack trace shows the token\n    being handed to google-auth-library's OAuth2Client.verifyIdTokenAsync /\n    verifySignedJwtWithCertsAsync inside a User.Auth handler. The API therefore\n    authenticates callers with\
  \ Google-issued OpenID Connect ID tokens (Google\n    Sign-In), verified server-side against Google's public certificates.\n  evidence:\n  - request: 'GET / with header \"Authorization: Bearer test\"'\n    status: 401\n    body_error: 'Wrong number of segments in token: test'\n    stack_frames:\n    - _OAuth2Client.verifySignedJwtWithCertsAsync\n    - _OAuth2Client.verifyIdTokenAsync\n    - User.Auth\ngate:\n  description: >-\n    Requests carrying no Authorization header are rejected by an application-level\n    gate before any token validation runs. The gate is not satisfied by any of the\n    common API-key header names probed (x-api-key, apikey, authorizationkey,\n    authorization-key), which all produced the same unauthenticated response.\n  status: 401\n  body: '{\"error\":\"authorization key is not provided\"}'\n  headers_probed_without_effect:\n  - x-api-key\n  - apikey\n  - authorizationkey\n  - authorization-key\ninfrastructure:\n  edge: Amazon CloudFront\n  gateway: AWS API\
  \ Gateway (HTTP API, $default stage, /{proxy+} catch-all route)\n  region: us-west-1\n  runtime: Node.js Lambda built with SST (apps/legacy/src/sst.mjs)\n  evidence:\n  - apigw-requestid + x-amzn-trace-id response headers\n  - via/x-amz-cf-id CloudFront response headers\n  - echoed requestContext.domainName aruc25yw2d.execute-api.us-west-1.amazonaws.com\naccess: private\nonboarding: >-\n  No public sign-up, key issuance or documentation surface was found. Access appears\n  to be granted only under a carrier or partner agreement; the Carrier Solutions page\n  describes the motion as \"Embed your products inside trusted partner ecosystems via\n  API\".\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amplify/refs/heads/main/authentication/amplify-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Insurance
- Insurtech
- Life Insurance
- Financial Services
- Fintech
- Embedded Finance
- Annuities
---
