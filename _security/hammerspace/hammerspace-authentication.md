---
api_key_in: []
auth_types:
- http
- session-cookie
- openIdConnect
description: ''
kind: authentication
layout: security
method: searched
name: Hammerspace Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- implicit
overview: Hammerspace secures its APIs with http, session-cookie, and openIdConnect across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and implicit flow(s).
provider_name: Hammerspace
provider_slug: hammerspace
scheme_count: 2
schemes:
- description: 'POST an application/x-www-form-urlencoded body with `username` and `password` to {anvil}/mgmt/v1.2/rest/login. A 200 establishes a session cookie that the client must carry (Hammerspace''s reference Go client uses a net/http cookiejar). Subsequent requests send Content-Type: application/json.'
  endpoint: https://{anvil-host}/mgmt/v1.2/rest/login
  name: anvil-form-login
  parameters:
  - in: formData
    name: username
  - in: formData
    name: password
  scheme: form-login
  session:
    mechanism: cookie
    reauthentication: Clients re-issue the login and retry once when a request returns 401 or 403; the reference driver does exactly this in doRequest.
  sources:
  - https://github.com/hammer-space/csi-plugin/blob/main/pkg/client/hsclient.go
  surface: apis.yml#hammerspace:anvil-management-api
  type: http
- authorization_endpoint: https://supportportal.hammerspace.com/services/oauth2/authorize
  description: Salesforce Experience Cloud identity for the Hammerspace customer support portal. Standard OIDC discovery is public; the endpoints below come verbatim from that document. This authenticates support-portal users, not the data platform API.
  end_session_endpoint: https://supportportal.hammerspace.com/services/auth/idp/oidc/logout
  id_token_signing_alg_values_supported:
  - RS256
  introspection_endpoint: https://supportportal.hammerspace.com/services/oauth2/introspect
  issuer: https://supportportal.hammerspace.com
  jwks_uri: https://supportportal.hammerspace.com/id/keys
  name: supportportal-oidc
  openIdConnectUrl: https://supportportal.hammerspace.com/.well-known/openid-configuration
  registration_endpoint: https://supportportal.hammerspace.com/services/oauth2/register
  revocation_endpoint: https://supportportal.hammerspace.com/services/oauth2/revoke
  scopes: scopes/hammerspace-scopes.yml
  sources:
  - well-known/hammerspace-openid-configuration.json
  surface: https://supportportal.hammerspace.com
  token_endpoint: https://supportportal.hammerspace.com/services/oauth2/token
  type: openIdConnect
  userinfo_endpoint: https://supportportal.hammerspace.com/services/oauth2/userinfo
slug: hammerspace-authentication
source_filename: hammerspace-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-04'\nmethod: searched\nsource: >-\n  Hammerspace's own Apache-2.0 open source clients (csi-plugin pkg/client and\n  deploy/kubernetes/SECRETS.md) plus the live OIDC discovery document on the\n  Hammerspace support portal. Hammerspace publishes no OpenAPI, so no\n  securityScheme block could be derived mechanically.\nsummary:\n  types: [http, session-cookie, openIdConnect]\n  api_key_in: []\n  oauth2_flows: [authorizationCode, implicit]\n  note: >-\n    Two distinct auth surfaces exist. The Anvil management REST API uses a form\n    login that establishes a session cookie — there is no API key, bearer token\n    or OAuth flow on that surface. The Salesforce Experience Cloud support portal\n    is a separate OIDC/OAuth2 identity surface for customer support, not for the\n    data platform API.\nschemes:\n- name: anvil-form-login\n  surface: apis.yml#hammerspace:anvil-management-api\n  type: http\n  scheme: form-login\n  description: >-\n    POST an application/x-www-form-urlencoded\
  \ body with `username` and `password`\n    to {anvil}/mgmt/v1.2/rest/login. A 200 establishes a session cookie that the\n    client must carry (Hammerspace's reference Go client uses a net/http\n    cookiejar). Subsequent requests send Content-Type: application/json.\n  endpoint: https://{anvil-host}/mgmt/v1.2/rest/login\n  parameters:\n  - name: username\n    in: formData\n  - name: password\n    in: formData\n  session:\n    mechanism: cookie\n    reauthentication: >-\n      Clients re-issue the login and retry once when a request returns 401 or\n      403; the reference driver does exactly this in doRequest.\n  sources:\n  - https://github.com/hammer-space/csi-plugin/blob/main/pkg/client/hsclient.go\n- name: supportportal-oidc\n  surface: https://supportportal.hammerspace.com\n  type: openIdConnect\n  openIdConnectUrl: https://supportportal.hammerspace.com/.well-known/openid-configuration\n  description: >-\n    Salesforce Experience Cloud identity for the Hammerspace customer support\n\
  \    portal. Standard OIDC discovery is public; the endpoints below come verbatim\n    from that document. This authenticates support-portal users, not the data\n    platform API.\n  issuer: https://supportportal.hammerspace.com\n  authorization_endpoint: https://supportportal.hammerspace.com/services/oauth2/authorize\n  token_endpoint: https://supportportal.hammerspace.com/services/oauth2/token\n  userinfo_endpoint: https://supportportal.hammerspace.com/services/oauth2/userinfo\n  jwks_uri: https://supportportal.hammerspace.com/id/keys\n  revocation_endpoint: https://supportportal.hammerspace.com/services/oauth2/revoke\n  introspection_endpoint: https://supportportal.hammerspace.com/services/oauth2/introspect\n  registration_endpoint: https://supportportal.hammerspace.com/services/oauth2/register\n  end_session_endpoint: https://supportportal.hammerspace.com/services/auth/idp/oidc/logout\n  id_token_signing_alg_values_supported: [RS256]\n  scopes: scopes/hammerspace-scopes.yml\n  sources:\n\
  \  - well-known/hammerspace-openid-configuration.json\nauthorization:\n  model: role-based ACLs per object type\n  description: >-\n    Hammerspace roles are per-object-type create/read/update/delete ACLs. A\n    service account can be bound to a custom role granting only the object types\n    an integration touches — Hammerspace's own CSI guidance recommends full\n    control of shares and snapshots plus read-only (R on ANY) everywhere else,\n    rather than a full Anvil administrator.\n  docs: https://github.com/hammer-space/csi-plugin/blob/main/deploy/kubernetes/SECRETS.md\ncredential_handling:\n  guidance_published: true\n  url: https://github.com/hammer-space/csi-plugin/blob/main/deploy/kubernetes/SECRETS.md\n  practices:\n  - Dedicated least-privilege Anvil service user rather than the admin account.\n  - Kubernetes Secret com.hammerspace.csi.credentials with username/password/endpoint\n    keys, injected via secretKeyRef.\n  - Documented Sealed Secrets, External Secrets Operator\
  \ and Secrets Store CSI paths.\n  - RBAC scoped to get on the single named Secret via resourceNames.\ntransport:\n  tls: required\n  note: >-\n    The reference client exposes a tlsVerify switch because Anvil deployments\n    frequently run with an internally issued certificate; verification is\n    enabled by default in the published manifests.\nfederation:\n  identity_providers: >-\n    The Anvil management API exposes /idp and /ad resources for configuring\n    external identity providers and Active Directory domain join, so directory\n    integration is a first-class configuration surface.\n  sources:\n  - https://github.com/hammer-space/ansible/blob/main/Operations/idp-add.yml\n  - https://github.com/hammer-space/ansible/blob/main/Operations/ad-join.yml\nx-evidence:\n  fetched: '2026-08-04'\n  probes:\n  - url: https://supportportal.hammerspace.com/.well-known/openid-configuration\n    http_status: 200\n    content_type: application/json;charset=UTF-8\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hammerspace/refs/heads/main/authentication/hammerspace-authentication.yml
summary_line: http/session-cookie/openIdConnect · 2 schemes
tags:
- Company
- Storage
- Data Management
- File Systems
- Data Orchestration
- Hybrid Cloud
- Kubernetes
- Artificial Intelligence
- Unstructured Data
- Infrastructure
---
