---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: probed
name: Level Home Authentication
name_suffix: Authentication
oauth_flows: []
overview: Level Home declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Level Home
provider_slug: level-home
scheme_count: 2
schemes:
- host: https://level.co/api/
  name: craft-public-schema
  observed: 'Anonymous POST returns data for the public schema (ping, globalSets, globalSet). Craft CMS private schemas are selected with an Authorization: Bearer <graphql-token> header, but Level publishes no token and no token-issuing surface.'
  type: none
- host: https://api.level.co
  name: unknown
  observed: No WWW-Authenticate challenge on 401/404 paths; unrouted paths return 404 rather than 401, so the authentication scheme is not externally observable. /.well-known/openid-configuration, /.well-known/oauth-authorization-server and /.well-known/oauth-protected-resource are all 404, so the backend advertises neither OIDC nor RFC 8414/9728 discovery.
  type: unknown
slug: level-home-authentication
source_filename: level-home-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-04'\nmethod: probed\nsource: live probes of https://level.co/api/ and https://api.level.co\ndocumented: false\nnote: >-\n  Level Home publishes no authentication documentation, no developer portal and no specification, so this\n  profile is observed rather than derived from securitySchemes. No `Authentication` pointer is wired into\n  apis.yml, because the scoring check that reads it asks whether the provider *documents* authentication,\n  and Level does not.\nsummary:\n  types: []\n  api_key_in: []\n  oauth2_flows: []\n  discovery_documents: none\nschemes:\n- host: https://level.co/api/\n  name: craft-public-schema\n  type: none\n  observed: >-\n    Anonymous POST returns data for the public schema (ping, globalSets, globalSet). Craft CMS private\n    schemas are selected with an Authorization: Bearer <graphql-token> header, but Level publishes no\n    token and no token-issuing surface.\n- host: https://api.level.co\n  name: unknown\n  type: unknown\n\
  \  observed: >-\n    No WWW-Authenticate challenge on 401/404 paths; unrouted paths return 404 rather than 401, so the\n    authentication scheme is not externally observable. /.well-known/openid-configuration,\n    /.well-known/oauth-authorization-server and /.well-known/oauth-protected-resource are all 404, so the\n    backend advertises neither OIDC nor RFC 8414/9728 discovery.\npublic_unauthenticated_routes:\n- path: /invite/{uuid}\n  note: Validates the UUID before auth; 400 on a malformed value.\n- path: /pass/{id}\n  note: Returns text/html — a guest-pass landing page.\n- path: /verify/{token}\n- path: /recover/{token}\n- path: /franklin/in-home/opt-in/{id}\nsource_of_routes: https://api.level.co/.well-known/apple-app-site-association\ngaps:\n- No published auth documentation for developers or partners.\n- No OAuth 2.0 / OIDC discovery.\n- No API key issuance surface.\n- Third-party access to Level devices is brokered by Seam rather than by a Level-issued credential.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/level-home/refs/heads/main/authentication/level-home-authentication.yml
summary_line: 2 schemes
tags:
- Smart Lock
- Smart Home
- Home Automation
- IoT
- Access Control
- Matter
- Thread
- Bluetooth LE
- apple-home-key
- Consumer Hardware
- Multifamily
- PropTech
- GraphQL
---
