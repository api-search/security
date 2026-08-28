---
api_key_in: []
api_specs:
- filename: nusano-posts-api-openapi.yml
  format: yaml
  label: Nusano Posts API
  slug: posts
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nusano/refs/heads/main/openapi/nusano-posts-api-openapi.yml
- filename: nusano-pages-api-openapi.yml
  format: yaml
  label: Nusano Pages API
  slug: pages
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nusano/refs/heads/main/openapi/nusano-pages-api-openapi.yml
- filename: nusano-media-api-openapi.yml
  format: yaml
  label: Nusano Media API
  slug: media
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nusano/refs/heads/main/openapi/nusano-media-api-openapi.yml
- filename: nusano-categories-api-openapi.yml
  format: yaml
  label: Nusano Categories API
  slug: categories
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nusano/refs/heads/main/openapi/nusano-categories-api-openapi.yml
- filename: nusano-tags-api-openapi.yml
  format: yaml
  label: Nusano Tags API
  slug: tags
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nusano/refs/heads/main/openapi/nusano-tags-api-openapi.yml
- filename: nusano-users-api-openapi.yml
  format: yaml
  label: Nusano Users API
  slug: users
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nusano/refs/heads/main/openapi/nusano-users-api-openapi.yml
- filename: nusano-comments-api-openapi.yml
  format: yaml
  label: Nusano Comments API
  slug: comments
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nusano/refs/heads/main/openapi/nusano-comments-api-openapi.yml
- filename: nusano-search-api-openapi.yml
  format: yaml
  label: Nusano Search API
  slug: search
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nusano/refs/heads/main/openapi/nusano-search-api-openapi.yml
- filename: nusano-discovery-api-openapi.yml
  format: yaml
  label: Nusano Discovery API
  slug: discovery
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nusano/refs/heads/main/openapi/nusano-discovery-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Nusano Authentication
name_suffix: Authentication
oauth_flows: []
overview: Nusano secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Nusano
provider_slug: nusano
scheme_count: 1
schemes:
- description: WordPress Application Passwords over HTTP Basic. Anonymous read is permitted on these routes; every write requires credentials.
  name: applicationPassword
  scheme: basic
  sources:
  - openapi/nusano-categories-api-openapi.yml
  - openapi/nusano-comments-api-openapi.yml
  - openapi/nusano-discovery-api-openapi.yml
  - openapi/nusano-media-api-openapi.yml
  - openapi/nusano-pages-api-openapi.yml
  - openapi/nusano-posts-api-openapi.yml
  - openapi/nusano-search-api-openapi.yml
  - openapi/nusano-tags-api-openapi.yml
  - openapi/nusano-users-api-openapi.yml
  type: http
slug: nusano-authentication
source_filename: nusano-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: derived\nsource: openapi/nusano-categories-api-openapi.yml, openapi/nusano-comments-api-openapi.yml, openapi/nusano-discovery-api-openapi.yml,\n  openapi/nusano-media-api-openapi.yml, openapi/nusano-pages-api-openapi.yml, openapi/nusano-posts-api-openapi.yml,\n  openapi/nusano-search-api-openapi.yml, openapi/nusano-tags-api-openapi.yml, openapi/nusano-users-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: applicationPassword\n  type: http\n  scheme: basic\n  description: WordPress Application Passwords over HTTP Basic. Anonymous read is permitted on these routes;\n    every write requires credentials.\n  sources:\n  - openapi/nusano-categories-api-openapi.yml\n  - openapi/nusano-comments-api-openapi.yml\n  - openapi/nusano-discovery-api-openapi.yml\n  - openapi/nusano-media-api-openapi.yml\n  - openapi/nusano-pages-api-openapi.yml\n  - openapi/nusano-posts-api-openapi.yml\n  - openapi/nusano-search-api-openapi.yml\n  - openapi/nusano-tags-api-openapi.yml\n\
  \  - openapi/nusano-users-api-openapi.yml\nnote: 'Nusano publishes no authentication documentation — there is no developer portal on nusano.com.\n  This profile was DERIVED from the specs in openapi/, which were themselves derived from the live WordPress\n  route index. It was then confirmed against live probes: anonymous GET on the wp/v2 content collections\n  returns 200, and every write plus the MCP and abilities endpoints return 401 with the WordPress rest_forbidden\n  envelope.'\nanonymous_read: true\nauthorization_endpoint: https://nusano.com/wp-admin/authorize-application.php\nauthorization_endpoint_source: https://nusano.com/wp-json/ (authentication.application-passwords.endpoints.authorization)\nself_service_signup: false\nprobes:\n- url: https://nusano.com/wp-json/wp/v2/posts?per_page=1\n  method: GET\n  auth: none\n  status: 200\n- url: https://nusano.com/wp-json/wp/v2/settings\n  method: GET\n  auth: none\n  status: 401\n  code: rest_forbidden\n- url: https://nusano.com/wp-json/mcp/mcp-adapter-default-server\n\
  \  method: POST tools/list\n  auth: none\n  status: 401\n  code: rest_forbidden\n- url: https://nusano.com/.well-known/openid-configuration\n  method: GET\n  auth: none\n  status: 404\n- url: https://nusano.com/.well-known/oauth-authorization-server\n  method: GET\n  auth: none\n  status: 404\noauth:\n  supported: false\n  note: No OAuth or OIDC metadata is served; no scopes/ artifact is emitted.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nusano/refs/heads/main/authentication/nusano-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Radioisotopes
- Nuclear Medicine
- Life Sciences
- Healthcare
- Oncology
- Radiopharmaceuticals
- Physics
- Advanced Manufacturing
- Nuclear Energy
- HALEU
- Critical Minerals
- Content
---
