---
anonymous_access: true
api_key_in: []
api_specs:
- filename: xgs-energy-posts-api-openapi.yml
  format: yaml
  label: XGS Energy Posts API
  slug: xgs-energy-posts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xgs-energy/refs/heads/main/openapi/xgs-energy-posts-api-openapi.yml
- filename: xgs-energy-pages-api-openapi.yml
  format: yaml
  label: XGS Energy Pages API
  slug: xgs-energy-pages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xgs-energy/refs/heads/main/openapi/xgs-energy-pages-api-openapi.yml
- filename: xgs-energy-media-api-openapi.yml
  format: yaml
  label: XGS Energy Media API
  slug: xgs-energy-media-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xgs-energy/refs/heads/main/openapi/xgs-energy-media-api-openapi.yml
- filename: xgs-energy-search-api-openapi.yml
  format: yaml
  label: XGS Energy Search API
  slug: xgs-energy-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xgs-energy/refs/heads/main/openapi/xgs-energy-search-api-openapi.yml
- filename: xgs-energy-categories-api-openapi.yml
  format: yaml
  label: XGS Energy Categories API
  slug: xgs-energy-categories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xgs-energy/refs/heads/main/openapi/xgs-energy-categories-api-openapi.yml
- filename: xgs-energy-tags-api-openapi.yml
  format: yaml
  label: XGS Energy Tags API
  slug: xgs-energy-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xgs-energy/refs/heads/main/openapi/xgs-energy-tags-api-openapi.yml
- filename: xgs-energy-discovery-api-openapi.yml
  format: yaml
  label: XGS Energy Discovery API
  slug: xgs-energy-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xgs-energy/refs/heads/main/openapi/xgs-energy-discovery-api-openapi.yml
- filename: xgs-energy-oembed-api-openapi.yml
  format: yaml
  label: XGS Energy oEmbed API
  slug: xgs-energy-oembed-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xgs-energy/refs/heads/main/openapi/xgs-energy-oembed-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: probed
name: Xgs Energy Authentication
name_suffix: Authentication
oauth_flows: []
overview: XGS Energy declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: XGS Energy
provider_slug: xgs-energy
scheme_count: 2
schemes:
- applies_to: all GET routes captured in openapi/
  description: 'No credential is sent or required. Verified live: GET /wp/v2/posts, /pages, /media, /search, /categories, /tags, /types, /taxonomies and /oembed/1.0/embed all returned 200 anonymously.'
  evidence: https://www.xgsenergy.com/wp-json/wp/v2/posts?per_page=1 -> 200
  id: anonymous
  type: none
- applies_to: write routes and privileged read contexts (not part of the public surface)
  authorization_endpoint: https://www.xgsenergy.com/wp-admin/authorize-application.php
  description: WordPress Application Passwords, advertised by the provider in the `authentication` block of the route index. Credentials are issued from the site's own wp-admin authorization screen, which is an administrator function, not a developer onboarding flow. No public route is documented as writable.
  evidence: https://www.xgsenergy.com/wp-json/
  id: application-passwords
  scheme: basic
  type: http
slug: xgs-energy-authentication
source_filename: xgs-energy-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-04'\nmethod: probed\nsource: https://www.xgsenergy.com/wp-json/\nprovider: XGS Energy\nsurface: WordPress REST API behind www.xgsenergy.com\nsummary: The entire public surface is anonymous and read-only. Every collection and item route captured in\n  openapi/ returned 200 to an unauthenticated GET on 2026-09-04. No API key, token, OAuth flow or signup exists\n  — there is no developer program to sign up to.\nschemes:\n- id: anonymous\n  type: none\n  applies_to: all GET routes captured in openapi/\n  description: 'No credential is sent or required. Verified live: GET /wp/v2/posts, /pages, /media, /search,\n    /categories, /tags, /types, /taxonomies and /oembed/1.0/embed all returned 200 anonymously.'\n  evidence: https://www.xgsenergy.com/wp-json/wp/v2/posts?per_page=1 -> 200\n- id: application-passwords\n  type: http\n  scheme: basic\n  applies_to: write routes and privileged read contexts (not part of the public surface)\n  description: WordPress Application\
  \ Passwords, advertised by the provider in the `authentication` block of\n    the route index. Credentials are issued from the site's own wp-admin authorization screen, which is an\n    administrator function, not a developer onboarding flow. No public route is documented as writable.\n  authorization_endpoint: https://www.xgsenergy.com/wp-admin/authorize-application.php\n  evidence: https://www.xgsenergy.com/wp-json/\ngated_surfaces:\n- path: /wp-json/wp/v2/settings\n  status: 401\n  code: rest_forbidden\n- path: /wp-json/wp/v2/menus\n  status: 401\n  code: rest_cannot_view\n- path: /wp-json/wp-abilities/v1/abilities\n  status: 401\n  code: rest_forbidden\n- path: /wp-json/hfe/v1/mcp-abilities\n  status: 403\n  code: uae_rest_not_allowed\n- path: /wp-json/contact-form-7/v1/contact-forms\n  status: 403\n  code: wpcf7_forbidden\noauth2: false\nopenid_connect: false\nmtls: false\napi_keys: false\nnotes:\n- No /.well-known/openid-configuration or /.well-known/oauth-authorization-server is\
  \ served (both 404, see\n  well-known/).\n- There is no signup, console, or key issuance page anywhere on xgsenergy.com.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/xgs-energy/refs/heads/main/authentication/xgs-energy-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Energy
- Geothermal
- Renewable Energy
- Clean Energy
- Power Generation
- Energy Infrastructure
- Data Center Power
- Climate Tech
- Content
---
