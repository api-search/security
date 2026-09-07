---
anonymous_access: false
api_key_in: []
api_specs:
- filename: webscale-networks-webscale-apis-openapi.json
  format: json
  label: Webscale APIs
  slug: webscale-apis
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/webscale-networks/refs/heads/main/openapi/webscale-networks-webscale-apis-openapi.json
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Webscale Networks Authentication
name_suffix: Authentication
oauth_flows: []
overview: Webscale Networks secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Webscale Networks
provider_slug: webscale-networks
scheme_count: 1
schemes:
- applied: 'globally via the root-level security: [{access_key: []}]'
  description_verbatim: An access key secret must be sent as a bearer token with each HTTP request in an `Authorization` header.
  name: access_key
  scheme: Bearer
  sources:
  - openapi/webscale-networks-webscale-apis-openapi.json
  - https://control.webscale.com/docs/api
  token_acquisition:
  - api: POST /users/{id}/access-keys
    how: Create an access key in your user profile.
    list: GET /users/{id}/access-keys
    method: user access key
    revoke: DELETE /users/{user_id}/access-keys/{id}
    url: https://control.webscale.com/profile
  - api: POST /accounts/{id}/service-users
    how: An access key secret created when a service user is created.
    method: service user secret
    note: The non-human/machine principal path. This is what an agent or CI job should use.
  - api: POST /users/{id}/authorization
    how: Obtain a temporary access key using an existing access key secret for a specified account.
    method: temporary access key
    note: The closest thing this API has to token exchange — a long-lived secret is traded for a short-lived, account-scoped token. The contract does not publish the resulting token's lifetime.
    read: GET /users/{id}/authorization
  transport:
    alternative:
      caution: A bearer token in a query string is written to access logs, proxy logs and browser history. Prefer the header. Recorded because the provider offers it, not because it is advisable.
      declared_at: components.parameters.authorization
      description_verbatim: Access token.  The authorization request header and this query parameter are exclusive. Exactly one must be provided.
      query_parameter: authorization
    primary:
      form: 'Authorization: Bearer <access-key-secret>'
      header: Authorization
      rfc: RFC 7235 section 5.1 (cited by the provider in the scheme description)
  type: http
slug: webscale-networks-authentication
source_filename: webscale-networks-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-04'\nmethod: searched\nsource: >-\n  openapi/webscale-networks-webscale-apis-openapi.json (components.securitySchemes.access_key) and\n  https://control.webscale.com/docs/api; live unauthenticated probes of https://api.webscale.com/v2\ndocs: https://control.webscale.com/docs/api\nname: Webscale APIs authentication\napi: Webscale APIs\nbase_url: https://api.webscale.com/v2\n\nsummary:\n  types:\n  - http\n  model: single bearer credential, applied globally\n  oauth2: false\n  oidc: false\n  mtls: false\n  api_key_header: false\n  scopes: none\n  mfa_for_api: not applicable (console MFA is documented separately)\n\nschemes:\n- name: access_key\n  type: http\n  scheme: Bearer\n  applied: 'globally via the root-level security: [{access_key: []}]'\n  transport:\n    primary:\n      header: Authorization\n      form: 'Authorization: Bearer <access-key-secret>'\n      rfc: RFC 7235 section 5.1 (cited by the provider in the scheme description)\n    alternative:\n\
  \      query_parameter: authorization\n      declared_at: components.parameters.authorization\n      description_verbatim: >-\n        Access token.  The authorization request header and this query parameter are exclusive.\n        Exactly one must be provided.\n      caution: >-\n        A bearer token in a query string is written to access logs, proxy logs and browser history.\n        Prefer the header. Recorded because the provider offers it, not because it is advisable.\n  description_verbatim: >-\n    An access key secret must be sent as a bearer token with each HTTP request in an `Authorization`\n    header.\n  token_acquisition:\n  - method: user access key\n    how: Create an access key in your user profile.\n    url: https://control.webscale.com/profile\n    api: POST /users/{id}/access-keys\n    list: GET /users/{id}/access-keys\n    revoke: DELETE /users/{user_id}/access-keys/{id}\n  - method: service user secret\n    how: An access key secret created when a service user is\
  \ created.\n    api: POST /accounts/{id}/service-users\n    note: The non-human/machine principal path. This is what an agent or CI job should use.\n  - method: temporary access key\n    how: >-\n      Obtain a temporary access key using an existing access key secret for a specified account.\n    api: POST /users/{id}/authorization\n    read: GET /users/{id}/authorization\n    note: >-\n      The closest thing this API has to token exchange — a long-lived secret is traded for a\n      short-lived, account-scoped token. The contract does not publish the resulting token's lifetime.\n  sources:\n  - openapi/webscale-networks-webscale-apis-openapi.json\n  - https://control.webscale.com/docs/api\n\nauthorization_model:\n  style: role and group based, managed through the API\n  objects:\n    roles: /accounts/{id}/roles\n    role_invitations: /accounts/{id}/invitations\n    groups: /accounts/{id}/groups\n    group_invitations: /accounts/{id}/group-invitations\n    user_role_membership: /users/{id}/roles,\
  \ /users/{id}/roles/{role_id}\n    user_group_membership: /users/{id}/groups, /users/{id}/groups/{group_id}\n    service_users: /accounts/{id}/service-users\n  scopes_published: false\n  permission_reference_published: false\n  finding: >-\n    Authorization is real and richly modelled — 20 operations across roles, groups, invitations and\n    memberships — but NO permission or scope reference is published. There is no document saying which\n    role grants which operation, and the contract attaches no per-operation scope requirement. A caller\n    cannot determine in advance whether a given key may perform a given call; they must attempt it.\n\ntoken_properties:\n  expiry_published: false\n  rotation_policy_published: false\n  revocation: DELETE /users/{user_id}/access-keys/{id}\n  prefix: none published\n  format: opaque secret\n\nobserved_runtime:\n  method: probed\n  probed: '2026-09-04'\n  unauthenticated_response:\n    status: 401\n    body: '{ \"status\": 401, \"error\": { \"type\"\
  : \"unauthorized\", \"message\": \"Your request must include an authorizationheader including a bearer token\" } }'\n    header_www_authenticate: not returned\n  control_probe: >-\n    A nonsense path (/v2/definitely-not-a-real-endpoint-9f3a) returns the identical 401 body as a real\n    path (/v2/applications). The API does not distinguish \"unauthenticated\" from \"not found\" to an\n    anonymous caller — an intentional non-enumeration posture.\n  note: >-\n    The live 401 body does not match the contract's declared `Error` schema. See\n    errors/webscale-networks-problem-types.yml.\n\ndiscovery_documents:\n  openid_configuration: not served (404 on webscale.com, api.webscale.com, docs.webscale.com)\n  oauth_authorization_server: not served\n  oauth_protected_resource: not served\n  note: See well-known/webscale-networks-well-known.yml for the full 48-probe record.\n\nconsole_security_docs:\n  mfa: https://docs.webscale.com/docs/how-tos/security/mfa/\n  secure_access: https://docs.webscale.com/docs/how-tos/security/secure-access/\n\
  \  password_guidance: https://docs.webscale.com/docs/how-tos/security/password-guidance/\n  note: These cover human console login, not API credentials.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/webscale-networks/refs/heads/main/authentication/webscale-networks-authentication.yml
summary_line: http · 1 scheme
tags:
- Ecommerce
- Cloud Hosting
- Content Delivery Network
- Application Delivery
- Web Application Firewall
- Edge Computing
- Managed Hosting
- Infrastructure
- Magento
- Adobe Commerce
- Observability
---
