---
anonymous_access: false
api_key_in: []
auth_types: []
description: MeisterTask API authentication uses OAuth 2.0 access tokens sent in the Bearer Authorization header. Personal access tokens can also be created without prior application registration.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Meistertask Authentication
name_suffix: Authentication
oauth_flows: []
overview: MeisterTask declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: MeisterTask
provider_slug: meistertask
scheme_count: 1
schemes:
- evidence: To authorize an API request the access token has to be sent in the bearer authorization header.
  flows:
  - authorization_code
  - implicit
  - client_credentials
  header: Authorization
  how_to_obtain: Register an OAuth 2.0 client application to obtain a client ID and a client secret. Use one of the supported OAuth 2.0 flows to receive an access token. Personal access tokens can also be created without prior application registration.
  location: header
  name: OAuth 2.0
  scopes:
  - userinfo.profile
  - userinfo.email
  - meistertask
  type: oauth2
slug: meistertask-authentication
source_filename: meistertask-authentication.yml
source_heading: Authentication Profile
source_url: https://developers.meistertask.com/reference/authentication
source_yaml: "generated: '2026-10-14'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://developers.meistertask.com/reference/authentication\nsources:\n- https://developers.meistertask.com/reference/authentication\ndescription: MeisterTask API authentication uses OAuth 2.0 access tokens sent in the Bearer Authorization header. Personal access tokens can also\n  be created without prior application registration.\nschemes:\n- type: oauth2\n  name: OAuth 2.0\n  evidence: To authorize an API request the access token has to be sent in the bearer authorization header.\n  location: header\n  header: Authorization\n  flows:\n  - authorization_code\n  - implicit\n  - client_credentials\n  scopes:\n  - userinfo.profile\n  - userinfo.email\n  - meistertask\n  how_to_obtain: Register an OAuth 2.0 client application to obtain a client ID and a client secret. Use one of the supported OAuth 2.0 flows\n    to receive an access token. Personal access tokens can also be created\
  \ without prior application registration.\ndocs: https://developers.meistertask.com/reference/authentication\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/meistertask/refs/heads/main/authentication/meistertask-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Software-as-a-Service
- Project Management
- Collaboration
- Productivity
---
