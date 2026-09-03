---
api_key_in: []
auth_types: []
description: 'Authentication posture across every Universiti Teknologi Malaysia surface reachable from the open internet. UTM has no public developer program, so there is no route by which an unaffiliated caller obtains a credential for anything. The pattern that emerges is a clean split: the harvesting protocols are fully anonymous and the REST interfaces beneath them are closed, and the one fully specified authorization server is a campus identity service whose clients are provisioned by hand.'
kind: authentication
layout: security
method: probed
name: Utm Authentication
name_suffix: Authentication
oauth_flows: []
overview: Universiti Teknologi Malaysia declares 5 security scheme(s) across its OpenAPI definitions.
provider_name: Universiti Teknologi Malaysia
provider_slug: utm
scheme_count: 5
schemes:
- authorization_endpoint: https://login.microsoftonline.com/9c827912-3502-4333-ba47-1b242c3d20e6/oauth2/v2.0/authorize
  campus_entry_point: https://my.utm.my/login
  client_auth_methods:
  - client_secret_post
  - client_secret_basic
  - private_key_jwt
  - self_signed_tls_client_auth
  device_authorization_endpoint: https://login.microsoftonline.com/9c827912-3502-4333-ba47-1b242c3d20e6/oauth2/v2.0/devicecode
  discovery: https://login.microsoftonline.com/utm.my/v2.0/.well-known/openid-configuration
  dynamic_client_registration: false
  end_session_endpoint: https://login.microsoftonline.com/9c827912-3502-4333-ba47-1b242c3d20e6/oauth2/v2.0/logout
  id_token_signing_algs:
  - RS256
  issuer: https://login.microsoftonline.com/9c827912-3502-4333-ba47-1b242c3d20e6/v2.0
  jwks_uri: https://login.microsoftonline.com/9c827912-3502-4333-ba47-1b242c3d20e6/discovery/v2.0/keys
  name: UTM federated identity (OpenID Connect / OAuth 2.0, Microsoft Entra ID)
  public_client_registration: false
  registration_note: The discovery document publishes no registration_endpoint. A client_id exists only if UTM Digital creates one inside the tenant, so this authorization server is readable by anyone and callable by nobody outside the institution.
  response_types:
  - code
  - id_token
  - code id_token
  - id_token token
  scopes:
  - openid
  - profile
  - email
  - offline_access
  subject_types:
  - pairwise
  token_endpoint: https://login.microsoftonline.com/9c827912-3502-4333-ba47-1b242c3d20e6/oauth2/v2.0/token
  type: openIdConnect
  userinfo_endpoint: https://graph.microsoft.com/oidc/userinfo
  x-operator: federation
- endpoint: https://utmik.utm.my/server/oai/request
  name: UTMIK Repository — anonymous OAI-PMH harvesting
  note: OAI-PMH 2.0 verbs (Identify, ListMetadataFormats, ListSets) answered anonymously with no credential, no key and no rate-limit header. This is the one interface on a UTM host that an unaffiliated machine can actually call today.
  status: 200
  type: none
  x-operator: institution
- endpoint: https://utmik.utm.my/server/api
  name: UTMIK Repository — DSpace-CRIS REST API
  note: The HAL root is anonymously readable and advertises `authn`, `authorizations`, `logins` and `oidc` link relations, but every collection endpoint beneath it — /core/communities, /core/items, /core/sites, /discover/search/objects, /authn/status, /config/properties — returned HTTP 403 with an Apache-generated body to this environment. DSpace-CRIS normally exposes anonymous read on these, so the 403 is an edge policy rather than the application's own authorization model. Recorded as closed because that is how it answers.
  status: 200
  type: apiKey
  x-operator: institution
- challenge_body: '{"error":"You are not authorized to access the requested resource.","errorMessage":""}'
  endpoint: https://journals.utm.my/{journal}/api/v1
  name: UTM Press journals — Open Journal Systems REST API v1
  note: PKP OJS 3.x publishes a versioned REST API per journal. UTM Press runs it and it answers, but it requires an API token issued from a journal manager account; UTM Press publishes no route to request one. The same platform's OAI-PMH interface at https://journals.utm.my/index/oai is fully anonymous.
  scheme: bearer
  status: 401
  type: http
  x-operator: institution
- endpoint: https://my.utm.my/login
  name: MyUTM Portal
  note: Laravel session login with a CSRF token, for staff and students. Human interface only; no documented machine interface behind it.
  status: 200
  type: session
  x-operator: institution
slug: utm-authentication
source_filename: utm-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-01'\nmethod: probed\nsource: >-\n  https://login.microsoftonline.com/utm.my/v2.0/.well-known/openid-configuration (200, JSON),\n  https://login.microsoftonline.com/9c827912-3502-4333-ba47-1b242c3d20e6/federationmetadata/2007-06/federationmetadata.xml\n  (200, 28,441 bytes XML),\n  https://login.microsoftonline.com/getuserrealm.srf?login=user@utm.my&json=1 (200),\n  https://utmik.utm.my/server/api (200, anonymous read),\n  https://utmik.utm.my/server/api/core/communities (403),\n  https://journals.utm.my/index.php/index/oai?verb=Identify (200, anonymous),\n  https://journals.utm.my/jurnalteknologi/api/v1/issues (401, application/json),\n  https://my.utm.my/login (200) — all fetched 2026-09-01\nprovider: Universiti Teknologi Malaysia\nproviderId: utm\ndescription: >-\n  Authentication posture across every Universiti Teknologi Malaysia surface reachable from the\n  open internet. UTM has no public developer program, so there is no route by which an\n  unaffiliated\
  \ caller obtains a credential for anything. The pattern that emerges is a clean\n  split: the harvesting protocols are fully anonymous and the REST interfaces beneath them are\n  closed, and the one fully specified authorization server is a campus identity service whose\n  clients are provisioned by hand.\n\nschemes:\n- name: UTM federated identity (OpenID Connect / OAuth 2.0, Microsoft Entra ID)\n  type: openIdConnect\n  x-operator: federation\n  issuer: https://login.microsoftonline.com/9c827912-3502-4333-ba47-1b242c3d20e6/v2.0\n  discovery: https://login.microsoftonline.com/utm.my/v2.0/.well-known/openid-configuration\n  jwks_uri: https://login.microsoftonline.com/9c827912-3502-4333-ba47-1b242c3d20e6/discovery/v2.0/keys\n  authorization_endpoint: https://login.microsoftonline.com/9c827912-3502-4333-ba47-1b242c3d20e6/oauth2/v2.0/authorize\n  token_endpoint: https://login.microsoftonline.com/9c827912-3502-4333-ba47-1b242c3d20e6/oauth2/v2.0/token\n  userinfo_endpoint: https://graph.microsoft.com/oidc/userinfo\n\
  \  end_session_endpoint: https://login.microsoftonline.com/9c827912-3502-4333-ba47-1b242c3d20e6/oauth2/v2.0/logout\n  device_authorization_endpoint: https://login.microsoftonline.com/9c827912-3502-4333-ba47-1b242c3d20e6/oauth2/v2.0/devicecode\n  scopes:\n  - openid\n  - profile\n  - email\n  - offline_access\n  response_types:\n  - code\n  - id_token\n  - code id_token\n  - id_token token\n  client_auth_methods:\n  - client_secret_post\n  - client_secret_basic\n  - private_key_jwt\n  - self_signed_tls_client_auth\n  id_token_signing_algs:\n  - RS256\n  subject_types:\n  - pairwise\n  dynamic_client_registration: false\n  public_client_registration: false\n  registration_note: >-\n    The discovery document publishes no registration_endpoint. A client_id exists only if UTM\n    Digital creates one inside the tenant, so this authorization server is readable by anyone\n    and callable by nobody outside the institution.\n  campus_entry_point: https://my.utm.my/login\n\n- name: UTMIK Repository\
  \ — anonymous OAI-PMH harvesting\n  type: none\n  x-operator: institution\n  endpoint: https://utmik.utm.my/server/oai/request\n  status: 200\n  note: >-\n    OAI-PMH 2.0 verbs (Identify, ListMetadataFormats, ListSets) answered anonymously with no\n    credential, no key and no rate-limit header. This is the one interface on a UTM host that\n    an unaffiliated machine can actually call today.\n\n- name: UTMIK Repository — DSpace-CRIS REST API\n  type: apiKey\n  x-operator: institution\n  endpoint: https://utmik.utm.my/server/api\n  status: 200\n  note: >-\n    The HAL root is anonymously readable and advertises `authn`, `authorizations`, `logins`\n    and `oidc` link relations, but every collection endpoint beneath it — /core/communities,\n    /core/items, /core/sites, /discover/search/objects, /authn/status, /config/properties —\n    returned HTTP 403 with an Apache-generated body to this environment. DSpace-CRIS normally\n    exposes anonymous read on these, so the 403 is an edge policy\
  \ rather than the application's\n    own authorization model. Recorded as closed because that is how it answers.\n\n- name: UTM Press journals — Open Journal Systems REST API v1\n  type: http\n  scheme: bearer\n  x-operator: institution\n  endpoint: https://journals.utm.my/{journal}/api/v1\n  status: 401\n  challenge_body: '{\"error\":\"You are not authorized to access the requested resource.\",\"errorMessage\":\"\"}'\n  note: >-\n    PKP OJS 3.x publishes a versioned REST API per journal. UTM Press runs it and it answers,\n    but it requires an API token issued from a journal manager account; UTM Press publishes no\n    route to request one. The same platform's OAI-PMH interface at\n    https://journals.utm.my/index/oai is fully anonymous.\n\n- name: MyUTM Portal\n  type: session\n  x-operator: institution\n  endpoint: https://my.utm.my/login\n  status: 200\n  note: >-\n    Laravel session login with a CSRF token, for staff and students. Human interface only; no\n    documented machine\
  \ interface behind it.\n\nunreachable:\n- endpoint: http://eprints.utm.my/cgi/oai2\n  status: 0\n  note: >-\n    Connection refused on both port 80 and port 443 from this environment, HTTP 522 through an\n    independent proxy, and ECONNREFUSED from a third egress. DNS resolves to 161.139.21.110 on\n    UTM's own allocation, so the name is still published; the service is not answering the\n    public internet. No authentication posture can be recorded for it.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/utm/refs/heads/main/authentication/utm-authentication.yml
summary_line: 5 schemes
tags:
- University
- Higher Education
- Education
- Public Research University
- Technical University
- Malaysia
- Research
- Open Access
- Institutional Repository
- Research Repository
- Scholarly Publishing
- OAI-PMH
- Identity Federation
- SAML
- Crossref
---
