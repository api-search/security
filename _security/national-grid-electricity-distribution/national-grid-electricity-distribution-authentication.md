---
api_key_in:
- header
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: National Grid Electricity Distribution Authentication
name_suffix: Authentication
oauth_flows: []
overview: National Grid Electricity Distribution secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: National Grid Electricity Distribution
provider_slug: national-grid-electricity-distribution
scheme_count: 1
schemes:
- expiry: not published (tokens are long-lived until revoked)
  format: Opaque JWT-shaped bearer string. NGED's own redacted cURL example begins "eyJ0eX....eyJqdX...", confirming the CKAN 2.9 JWT-encoded API token format.
  in: header
  issuance: 'Self-issued from the signed-in user''s own profile: My User Profile -> "API Tokens" tab -> name the token -> "Create API Token". The value is displayed exactly once and cannot be retrieved again.'
  name: CKAN API Token
  parameter_name: Authorization
  prefix_note: 'The raw token value is sent as the entire Authorization header value. NGED''s published example uses NO "Bearer" prefix — `curl -H "Authorization: eyJ0eX..."`.'
  prefix_required: false
  revocation: Revoke by clicking the red "X" in the token's row in the API Tokens table on the user profile. NGED advises deleting rather than abandoning a lost token.
  rotation_policy: not published
  scopes: none — CKAN API tokens are not scoped; they carry the issuing user's permissions
  sources:
  - https://connecteddata.nationalgrid.co.uk/api-guidance
  type: apiKey
slug: national-grid-electricity-distribution-authentication
source_filename: national-grid-electricity-distribution-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-27'\nmethod: searched\nsource: https://connecteddata.nationalgrid.co.uk/api-guidance\ndocs: https://connecteddata.nationalgrid.co.uk/api-guidance\nnote: >-\n  Derived from NGED's own published API Guidance page plus live anonymous probes\n  of the CKAN Action API on 2026-07-27. There is no OpenAPI to derive\n  securitySchemes from, so every field below is grounded in the documentation\n  NGED publishes or in an observed response.\nsummary:\n  types: [apiKey]\n  api_key_in: [header]\n  oauth2_flows: []\n  anonymous_access: true\n  registration: self-serve\nschemes:\n- name: CKAN API Token\n  type: apiKey\n  in: header\n  parameter_name: Authorization\n  format: >-\n    Opaque JWT-shaped bearer string. NGED's own redacted cURL example begins\n    \"eyJ0eX....eyJqdX...\", confirming the CKAN 2.9 JWT-encoded API token format.\n  prefix_required: false\n  prefix_note: >-\n    The raw token value is sent as the entire Authorization header value. NGED's\n    published\
  \ example uses NO \"Bearer\" prefix — `curl -H \"Authorization: eyJ0eX...\"`.\n  issuance: >-\n    Self-issued from the signed-in user's own profile: My User Profile -> \"API\n    Tokens\" tab -> name the token -> \"Create API Token\". The value is displayed\n    exactly once and cannot be retrieved again.\n  revocation: >-\n    Revoke by clicking the red \"X\" in the token's row in the API Tokens table on\n    the user profile. NGED advises deleting rather than abandoning a lost token.\n  rotation_policy: not published\n  expiry: not published (tokens are long-lived until revoked)\n  scopes: none — CKAN API tokens are not scoped; they carry the issuing user's permissions\n  sources: [https://connecteddata.nationalgrid.co.uk/api-guidance]\nanonymous_surface:\n  description: >-\n    A large part of the API answers with no credential at all. These calls were\n    executed anonymously and returned HTTP 200 with success:true on 2026-07-27.\n  actions: [status_show, site_read, package_list,\
  \ package_search, package_show,\n    group_list, group_show, tag_list, tag_show, organization_list, license_list,\n    help_show]\n  catalogue_exports: [/catalog.jsonld, /catalog.ttl, /catalog.rdf, /catalog.n3]\n  resource_payloads: >-\n    778 of 8,691 resources expose a real download URL anonymously; the other\n    7,913 return the literal string \"redacted\" in place of the URL.\ngated_surface:\n  description: >-\n    Resource-level actions require a token. Observed anonymously, they return\n    HTTP 200/403 with success:false and an Authorization Error.\n  actions: [resource_show, datastore_search, user_list]\n  observed_response: >-\n    {\"error\": {\"__type\": \"Authorization Error\", \"message\": \"Access denied:\n    Resource access restricted to registered users\"}, \"success\": false}\n  restricted_levels_observed:\n    registered: 7911\n    public: 260\n    only_allowed_users: 2\n    unset: 518\n  note: >-\n    restricted_level is set per resource by the CKAN restricted_api\
  \ /\n    wpd_restricted_api extensions. \"registered\" is lifted by any verified\n    account; \"only_allowed_users\" is a named allow-list (2 resources).\nregistration_path:\n- step: 1\n  name: Anonymous\n  requirement: none\n  gets: full catalogue metadata, DCAT exports, 778 open resource payloads\n- step: 2\n  name: Register\n  url: https://connecteddata.nationalgrid.co.uk/user/register\n  requirement: email address plus an emailed verification code (links expire after 1 day)\n  approval: none — no accreditation, no organisation check, no licence signature\n- step: 3\n  name: Create an API token\n  url: https://connecteddata.nationalgrid.co.uk/user/login\n  requirement: signed-in session\n  gets: resource_show, datastore_search, and the 7,913 redacted download URLs\nnot_supported:\n  oauth2: >-\n    No OAuth 2.0 anywhere. /.well-known/oauth-authorization-server is 403 at the\n    edge on every NGED host.\n  openid_connect: >-\n    No OIDC. /.well-known/openid-configuration is 403 on\
  \ both\n    connecteddata.nationalgrid.co.uk and www.nationalgrid.co.uk.\n  mutual_tls: not offered\n  hmac_signing: not offered\ntransport_security:\n  https_only: true\n  tls_version: TLSv1.3\n  hsts: true\n  hsts_max_age: 31536000\n  see: security/national-grid-electricity-distribution-domain-security.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/national-grid-electricity-distribution/refs/heads/main/authentication/national-grid-electricity-distribution-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Energy
- United Kingdom
- Utilities
- Electricity
- Grid
- Distribution Network
- Open Data
- Smart Metering
- DER
- Flexibility
- Renewables
---
