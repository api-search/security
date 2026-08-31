---
api_key_in:
- query
api_specs:
- filename: validic-devices-api-openapi.yml
  format: yaml
  label: Validic Devices API
  slug: validic-devices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/validic/refs/heads/main/openapi/validic-devices-api-openapi.yml
- filename: validic-marketplace-connections-api-openapi.yml
  format: yaml
  label: Validic Marketplace & Connections API
  slug: validic-marketplace-connections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/validic/refs/heads/main/openapi/validic-marketplace-connections-api-openapi.yml
- filename: validic-observations-data-api-openapi.yml
  format: yaml
  label: Validic Observations & Data API
  slug: validic-observations-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/validic/refs/heads/main/openapi/validic-observations-data-api-openapi.yml
- filename: validic-push-service-api-openapi.yml
  format: yaml
  label: Validic Push Service API
  slug: validic-push-service-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/validic/refs/heads/main/openapi/validic-push-service-api-openapi.yml
- filename: validic-streaming-api-openapi.yml
  format: yaml
  label: Validic Streaming API
  slug: validic-streaming-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/validic/refs/heads/main/openapi/validic-streaming-api-openapi.yml
- filename: validic-users-api-openapi.yml
  format: yaml
  label: Validic Users API
  slug: validic-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/validic/refs/heads/main/openapi/validic-users-api-openapi.yml
- filename: validic-measurements-api-openapi.yml
  format: yaml
  label: Validic Measurements API
  slug: validic-measurements-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/validic/refs/heads/main/openapi/validic-measurements-api-openapi.yml
- filename: validic-organizations-api-openapi.yml
  format: yaml
  label: Validic Organizations API
  slug: validic-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/validic/refs/heads/main/openapi/validic-organizations-api-openapi.yml
- filename: validic-streams-api-openapi.yml
  format: yaml
  label: Validic Streams API
  slug: validic-streams-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/validic/refs/heads/main/openapi/validic-streams-api-openapi.yml
- filename: validic-streams-token-token-api-openapi.yml
  format: yaml
  label: Validic Streams?token={token} API
  slug: validic-streams-token-token-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/validic/refs/heads/main/openapi/validic-streams-token-token-api-openapi.yml
auth_types:
- apiKey
- http
description: Validic runs TWO different authentication models on two different hosts, and they must not be confused. The Inform data platform (REST + Streaming) uses a static organization access token in a QUERY PARAMETER. The developer signup API on api.dashboard.validic.com uses a bearer-style Authorization header carrying a Cognito-shaped id_token. Nothing bridges them - the signup tokens cannot call Inform, and the org token cannot call signup.
kind: authentication
layout: security
method: searched
name: Validic Authentication
name_suffix: Authentication
oauth_flows: []
overview: Validic secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Validic
provider_slug: validic
scheme_count: 2
schemes:
- applies_to: Validic Inform API (REST + Streaming)
  description: Organization access token passed as the `token` query parameter over HTTPS.
  expiry: none documented (static, long-lived)
  header_alternative: false
  header_note: 'There is no Authorization-header option. Validic''s own agent guide spells it out - "(query param, not a header)" - and warns the token will land in URLs, server logs, browser history and any copied curl command, so it must be handled like a password. This is the weakest part of the security posture and it is structural, not incidental: a PHI-bearing credential travelling in a query string cannot be kept out of intermediary logs.'
  hosts:
  - https://api.v2.validic.com
  - https://streams.v2.validic.com
  in: query
  name: tokenAuth
  obtained_from: https://dashboard.validic.com (Org ID and Org Token both shown)
  parameter: token
  required_on: every request
  rotation_documented: false
  scope: Bound to exactly one organization. Presenting it against a different org_id returns 401 "Token is not authorized to access organization". Within its organization it can read EVERY user - there is no per-user credential and no way to narrow it.
  sources:
  - openapi/_original/validic-inform-data-resources-openapi.json
  - openapi/_original/validic-streaming-resources-openapi.json
  - https://dashboard.validic.com/inform-quickstart.txt
  spec_defect: 'The published inform-data-resources spec declares this scheme with `name: api_key`, but every documented request, every example and the live API use `token`. A client generated straight from the spec would send the wrong parameter name. Corrected in overlays/validic-inform-data-resources-overlay.yaml, not in the original.'
  type: apiKey
- applies_to: Validic Developer Signup API
  discovery_document: none
  discovery_probe:
  - status: 403
    url: https://api.dashboard.validic.com/.well-known/openid-configuration
  - status: 403
    url: https://dashboard.validic.com/.well-known/openid-configuration
  hosts:
  - https://api.dashboard.validic.com
  identity_provider: Not named by Validic, but the three-token response shape, the register/verify/login sequence, the 6-digit email verification code and the `user_sub` field are all AWS Cognito conventions. Recorded as an observation, not a claim.
  in: header
  name: signupBearer
  note: OIDC-shaped tokens with no OIDC discovery document. An agent cannot validate the id_token's signature or issuer from anything Validic publishes.
  parameter: Authorization
  password_policy: Minimum 8 characters including uppercase, lowercase, a number and a special character.
  scheme: bearer
  sources:
  - https://dashboard.validic.com/validic-developer-signup.txt
  token_set:
  - id_token
  - access_token
  - refresh_token
  type: http
  value: the `id_token` returned by POST /auth/login
slug: validic-authentication
source_filename: validic-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-15'\nmethod: searched\nsource: >-\n  https://developer.validic.com/docs/requesting-access-to-data +\n  https://developer.validic.com/docs/inform-rest-api +\n  https://dashboard.validic.com/inform-quickstart.txt +\n  https://dashboard.validic.com/validic-developer-signup.txt +\n  openapi/_original/validic-inform-data-resources-openapi.json +\n  openapi/_original/validic-streaming-resources-openapi.json\ndocs: https://developer.validic.com/docs/requesting-access-to-data\ndescription: >-\n  Validic runs TWO different authentication models on two different hosts, and\n  they must not be confused. The Inform data platform (REST + Streaming) uses a\n  static organization access token in a QUERY PARAMETER. The developer signup\n  API on api.dashboard.validic.com uses a bearer-style Authorization header\n  carrying a Cognito-shaped id_token. Nothing bridges them - the signup tokens\n  cannot call Inform, and the org token cannot call signup.\nsummary:\n  types:\n\
  \  - apiKey\n  - http\n  api_key_in:\n  - query\n  oauth2: false\n  openid_connect: false\n  mutual_tls: false\n  scopes: false\n  mfa_on_api: false\nschemes:\n- name: tokenAuth\n  applies_to: Validic Inform API (REST + Streaming)\n  hosts:\n  - https://api.v2.validic.com\n  - https://streams.v2.validic.com\n  type: apiKey\n  in: query\n  parameter: token\n  required_on: every request\n  rotation_documented: false\n  expiry: none documented (static, long-lived)\n  scope: >-\n    Bound to exactly one organization. Presenting it against a different\n    org_id returns 401 \"Token is not authorized to access organization\".\n    Within its organization it can read EVERY user - there is no per-user\n    credential and no way to narrow it.\n  obtained_from: https://dashboard.validic.com (Org ID and Org Token both shown)\n  description: >-\n    Organization access token passed as the `token` query parameter over HTTPS.\n  sources:\n  - openapi/_original/validic-inform-data-resources-openapi.json\n\
  \  - openapi/_original/validic-streaming-resources-openapi.json\n  - https://dashboard.validic.com/inform-quickstart.txt\n  spec_defect: >-\n    The published inform-data-resources spec declares this scheme with\n    `name: api_key`, but every documented request, every example and the live\n    API use `token`. A client generated straight from the spec would send the\n    wrong parameter name. Corrected in\n    overlays/validic-inform-data-resources-overlay.yaml, not in the original.\n  header_alternative: false\n  header_note: >-\n    There is no Authorization-header option. Validic's own agent guide spells\n    it out - \"(query param, not a header)\" - and warns the token will land in\n    URLs, server logs, browser history and any copied curl command, so it must\n    be handled like a password. This is the weakest part of the security\n    posture and it is structural, not incidental: a PHI-bearing credential\n    travelling in a query string cannot be kept out of intermediary logs.\n\
  - name: signupBearer\n  applies_to: Validic Developer Signup API\n  hosts:\n  - https://api.dashboard.validic.com\n  type: http\n  scheme: bearer\n  in: header\n  parameter: Authorization\n  value: the `id_token` returned by POST /auth/login\n  token_set:\n  - id_token\n  - access_token\n  - refresh_token\n  identity_provider: >-\n    Not named by Validic, but the three-token response shape, the\n    register/verify/login sequence, the 6-digit email verification code and the\n    `user_sub` field are all AWS Cognito conventions. Recorded as an\n    observation, not a claim.\n  discovery_document: none\n  discovery_probe:\n  - url: https://api.dashboard.validic.com/.well-known/openid-configuration\n    status: 403\n  - url: https://dashboard.validic.com/.well-known/openid-configuration\n    status: 403\n  note: >-\n    OIDC-shaped tokens with no OIDC discovery document. An agent cannot\n    validate the id_token's signature or issuer from anything Validic\n    publishes.\n  sources:\n \
  \ - https://dashboard.validic.com/validic-developer-signup.txt\n  password_policy: >-\n    Minimum 8 characters including uppercase, lowercase, a number and a special\n    character.\noauth:\n  customer_facing: false\n  internal: true\n  note: >-\n    OAuth 2.0 is central to how the product WORKS but is never exposed to the\n    customer. The hosted Marketplace runs the OAuth authorization dance against\n    Fitbit, Garmin, Dexcom, Withings, Oura and the rest on the end user's\n    behalf, and the resulting grants are what make data flow. Validic\n    absorbs all of that so its customer never handles a third-party token -\n    which is a genuine part of the value, and also why there is no scope\n    surface for us to catalogue. scopes/ is deliberately not written.\nend_user_consent:\n  mechanism: hosted Marketplace (per-user, per-source)\n  revocation: >-\n    The user disconnects a source from the same Marketplace surface. Validic\n    tells integrators to keep a route back to it for\
  \ exactly this reason.\n  signal: >-\n    Connect and disconnect both emit a `connection` event on the Streaming API\n    and are retrievable over REST at /organizations/{org_id}/connections.\n  see: components/validic-components.yml\nphi_handling:\n  identifier_constraint: >-\n    The customer-defined `uid` travels in URLs and must therefore contain no\n    identifying data - no SSN, name, phone number or email address. Validic\n    states this as a HIPAA requirement on the integrator.\n  retention: 1 year retrievable via API; 7 years retained for compliance\ntransport:\n  https_required: true\n  tls_observed:\n  - host: api.v2.validic.com\n    tls: TLSv1.2\n  - host: developer.validic.com\n    tls: TLSv1.3\n  - host: validic.com\n    tls: TLSv1.3\n  see: security/validic-domain-security.yml\ngaps:\n- No Authorization-header option on the data API; the credential is always in the URL.\n- No documented token rotation, expiry or revocation procedure for the organization token.\n- No per-user\
  \ or per-scope credential - the org token reads every patient in the organization.\n- No OIDC discovery document despite issuing OIDC-shaped tokens on the signup API.\n- No mTLS option for a platform carrying PHI.\nmaintainers:\n- FN: Kin Lane\n  email: kin@apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/validic/refs/heads/main/authentication/validic-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Health Data
- Digital Health
- Wearables
- Remote Patient Monitoring
- Health IoT
- Interoperability
- HIPAA
---
