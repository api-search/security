---
api_key_in: []
auth_types: []
description: Authentication profile for the two EMC management APIs in this profile. Both are customer-hosted appliance APIs, so there is no EMC-operated authorization server, no OAuth, and no developer-portal API key. Authentication is HTTP Basic against the customer's own array, exchanged for a session token. The mechanics below are read from EMC's own shipped client code rather than from prose, because the reference documentation on developer.dell.com is behind an authenticated portal API.
kind: authentication
layout: security
method: searched
name: Emc Authentication
name_suffix: Authentication
oauth_flows: []
overview: EMC declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: EMC
provider_slug: emc
scheme_count: 0
schemes: []
slug: emc-authentication
source_filename: emc-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-29'\nmethod: searched\nsource: >-\n  https://github.com/EMCECS/python-ecsclient (ecsclient/baseclient.py,\n  ecsclient/common/token_request.py) and https://github.com/dell/PyU4V\n  (PyU4V/rest_requests.py, PyU4V/univmax_conn.py, PyU4V/version.py) — EMC's own\n  first-party client libraries, read on 2026-08-29.\nprovider: EMC\nproviderId: emc\ndescription: >-\n  Authentication profile for the two EMC management APIs in this profile. Both are\n  customer-hosted appliance APIs, so there is no EMC-operated authorization server, no\n  OAuth, and no developer-portal API key. Authentication is HTTP Basic against the\n  customer's own array, exchanged for a session token. The mechanics below are read from\n  EMC's own shipped client code rather than from prose, because the reference\n  documentation on developer.dell.com is behind an authenticated portal API.\nno_oauth_note: >-\n  Neither API declares an OAuth 2.0 or OpenID Connect flow, and no /.well-known/\n \
  \ oauth-authorization-server or openid-configuration document is served on any EMC or\n  Dell host probed (see well-known/emc-well-known.yml). No scopes/ artifact is written:\n  there is no scope surface to record, and an empty OAuthScopes file would be a false\n  claim of an authorization model these APIs do not have.\napis:\n  - api: EMC ECS Management REST API\n    schemes:\n      - id: ecs_basic_login\n        type: http\n        scheme: basic\n        in: header\n        header: Authorization\n        applies_to: The login exchange only\n        description: >-\n          A username and password are sent as HTTP Basic credentials to the ECS login\n          endpoint. The credentials are never used on subsequent resource calls.\n      - id: ecs_sds_auth_token\n        type: apiKey\n        in: header\n        header: X-SDS-AUTH-TOKEN\n        applies_to: Every ECS Management API call after login\n        description: >-\n          The login response returns the session token in the\
  \ `x-sds-auth-token` RESPONSE\n          header. Clients read it off the response headers and replay it as the\n          `X-SDS-AUTH-TOKEN` REQUEST header on every subsequent call. The header name is\n          case-insensitive in practice — EMC's own client writes it lowercase when\n          reading and uppercase when sending.\n    session:\n      login: GET /login\n      logout: GET /logout\n      logout_force_param: >-\n        `force=true` terminates every simultaneous session for the current user, not just\n        the calling one.\n      whoami: GET /user/whoami\n      token_lifetime: >-\n        Not published. EMC's client does not encode an expiry; it caches the token to\n        disk and re-authenticates when a validation call returns 401, 403 or 415.\n      revalidation_signal: >-\n        HTTP 401, 403 or 415 on a token-validation call means \"token stale, fetch a new\n        one\". HTTP 500 or anything else is raised as an error rather than retried.\n    additional_headers:\n\
  \      - name: X-EMC-Override\n        required: false\n        description: >-\n          Optional override header exposed by EMC's client as `override_header`. Used to\n          force operations the API would otherwise refuse.\n      - name: Accept\n        required: true\n        value: application/json\n    transport:\n      tls: required\n      port: 4443\n      certificate_note: >-\n        EMC's own client defaults `verify_ssl=False` and explicitly disables urllib3\n        warnings, because ECS appliances ship with self-signed certificates by default.\n        This is a real posture finding, not a recommendation: the shipped default for the\n        first-party client is to not verify the array's certificate.\n  - api: EMC Unisphere REST API\n    schemes:\n      - id: unisphere_basic\n        type: http\n        scheme: basic\n        in: header\n        header: Authorization\n        applies_to: Every Unisphere for PowerMax REST call\n        description: >-\n          PyU4V\
  \ uses requests.auth.HTTPBasicAuth against the Unisphere server for the\n          standard flow.\n      - id: unisphere_bearer\n        type: http\n        scheme: bearer\n        in: header\n        header: Authorization\n        applies_to: Token-based sessions\n        description: >-\n          When a token is supplied, PyU4V applies `Authorization: Bearer <token>` to the\n          base headers so it persists across the session. Both models are supported by the\n          same client.\n    session:\n      style: persistent REST session established per connection\n      api_version: >-\n        Unisphere API version 104 (Unisphere 10.4.0), pinned in the client and overridable\n        per connection via `u4v_version`.\n    transport:\n      tls: required\n      port: 8443\n      base_paths:\n        - /univmax/restapi\n        - /univmax/rest\ngaps:\n  - >-\n    No published OpenAPI declares these schemes. The profile is reconstructed from EMC's\n    shipped client code; an agent\
  \ cannot discover it from a machine-readable contract.\n  - >-\n    No token lifetime, refresh endpoint or rotation policy is published for the ECS\n    X-SDS-AUTH-TOKEN. Clients discover expiry only by receiving a 401.\n  - >-\n    No MFA, mTLS or certificate-bound token option is documented for either API.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/emc/refs/heads/main/authentication/emc-authentication.yml
summary_line: 0 schemes
tags:
- Cloud Infrastructure
- Data Management
- Data Protection
- Enterprise Storage
- Object Storage
- Storage
- S3 Compatible
- Fortune 500
---
