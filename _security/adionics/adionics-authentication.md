---
anonymous_access: false
api_key_in: []
api_specs:
- filename: adionics-posts-api-openapi.yml
  format: yaml
  label: Adionics Posts API
  slug: adionics-posts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adionics/refs/heads/main/openapi/adionics-posts-api-openapi.yml
- filename: adionics-pages-api-openapi.yml
  format: yaml
  label: Adionics Pages API
  slug: adionics-pages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adionics/refs/heads/main/openapi/adionics-pages-api-openapi.yml
- filename: adionics-media-api-openapi.yml
  format: yaml
  label: Adionics Media API
  slug: adionics-media-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adionics/refs/heads/main/openapi/adionics-media-api-openapi.yml
- filename: adionics-taxonomy-api-openapi.yml
  format: yaml
  label: Adionics Taxonomy API
  slug: adionics-taxonomy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adionics/refs/heads/main/openapi/adionics-taxonomy-api-openapi.yml
- filename: adionics-search-api-openapi.yml
  format: yaml
  label: Adionics Search API
  slug: adionics-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adionics/refs/heads/main/openapi/adionics-search-api-openapi.yml
- filename: adionics-discovery-api-openapi.yml
  format: yaml
  label: Adionics Discovery API
  slug: adionics-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adionics/refs/heads/main/openapi/adionics-discovery-api-openapi.yml
auth_types:
- none
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: probed
name: Adionics Authentication
name_suffix: Authentication
oauth_flows: []
overview: Adionics secures its APIs with none and http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Adionics
provider_slug: adionics
scheme_count: 1
schemes:
- applies_to:
  - /wp/v2/settings
  - /wp/v2/plugins
  - /wp/v2/themes
  - /wp/v2/elementor_library
  - /wp-abilities/v1/abilities
  - /mcp/mcp-adapter-default-server
  - any request with context=edit
  authorization_endpoint: https://www.adionics.com/wp-admin/authorize-application.php
  description: The only authentication mechanism the install advertises. The REST route index declares `authentication.application-passwords.endpoints.authorization`, pointing at https://www.adionics.com/wp-admin/authorize-application.php. Credentials are issued to existing WordPress users from wp-admin and presented as HTTP Basic. There is no self-service signup, no public registration, and no developer program — an application password can only be created by someone who already holds an Adionics WordPress account.
  name: WordPress Application Passwords
  scheme: basic
  source: https://www.adionics.com/wp-json/
  type: http
slug: adionics-authentication
source_filename: adionics-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-07'\nmethod: probed\nsource: >-\n  Live probes of https://www.adionics.com/wp-json/ on 2026-09-07 — the REST route index's\n  `authentication` member, plus observed anonymous responses on public and gated routes.\nsummary:\n  types:\n  - none\n  - http\n  api_key_in: []\n  oauth2_flows: []\n  note: >-\n    Adionics publishes no developer authentication documentation of any kind. The surface below was\n    established entirely by probing the live WordPress REST API behind www.adionics.com.\npublic_surface:\n  authentication: none\n  description: >-\n    The published read surface — posts, pages, media, categories, tags, search, users, types,\n    statuses, taxonomies, the route index, the Polylang language registry and the oEmbed endpoint —\n    returns HTTP 200 to a completely anonymous client. No key, token, cookie or nonce is required\n    and none is accepted for additional access.\n  verified: '2026-09-07'\nschemes:\n- name: WordPress Application Passwords\n\
  \  type: http\n  scheme: basic\n  description: >-\n    The only authentication mechanism the install advertises. The REST route index declares\n    `authentication.application-passwords.endpoints.authorization`, pointing at\n    https://www.adionics.com/wp-admin/authorize-application.php. Credentials are issued to existing\n    WordPress users from wp-admin and presented as HTTP Basic. There is no self-service signup, no\n    public registration, and no developer program — an application password can only be created by\n    someone who already holds an Adionics WordPress account.\n  authorization_endpoint: https://www.adionics.com/wp-admin/authorize-application.php\n  source: https://www.adionics.com/wp-json/\n  applies_to:\n  - /wp/v2/settings\n  - /wp/v2/plugins\n  - /wp/v2/themes\n  - /wp/v2/elementor_library\n  - /wp-abilities/v1/abilities\n  - /mcp/mcp-adapter-default-server\n  - any request with context=edit\ngated_observations:\n- path: /wp-json/mcp/mcp-adapter-default-server\n\
  \  method: POST\n  body: '{\"jsonrpc\":\"2.0\",\"id\":1,\"method\":\"tools/list\"}'\n  status: 401\n  code: rest_forbidden\n  note: The MCP endpoint is served but every JSON-RPC method is gated behind the same WordPress user check.\n- path: /wp-json/wp-abilities/v1/abilities\n  status: 401\n  code: rest_forbidden\n- path: /wp-json/wp/v2/settings\n  status: 401\n  code: rest_forbidden\nerror_envelope:\n  shape: WordPress REST error\n  example:\n    code: rest_forbidden\n    message: \"Désolé, vous n’avez pas l’autorisation de faire cela.\"\n    data:\n      status: 401\n  note: >-\n    Denials are returned with HTTP status 401 and a `code` of `rest_forbidden`. Messages are\n    localised to French even on the English site.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/adionics/refs/heads/main/authentication/adionics-authentication.yml
summary_line: none/http · 1 scheme
tags:
- Company
- Cleantech
- Lithium
- Direct Lithium Extraction
- Mining
- Battery Materials
- Water Treatment
- Desalination
- Geothermal
- Industrial Process Technology
- Sustainability
- Content
---
