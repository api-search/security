---
api_key_in:
- cookie
api_specs:
- filename: caamtech-akismet-v1-api-openapi.yml
  format: yaml
  label: CaaMTech Akismet/v1 API
  slug: caamtech-akismet-v1-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/caamtech/refs/heads/main/openapi/caamtech-akismet-v1-api-openapi.yml
- filename: caamtech-mcp-api-openapi.yml
  format: yaml
  label: CaaMTech MCP API
  slug: caamtech-mcp-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/caamtech/refs/heads/main/openapi/caamtech-mcp-api-openapi.yml
- filename: caamtech-objectcache-v1-api-openapi.yml
  format: yaml
  label: CaaMTech Objectcache/v1 API
  slug: caamtech-objectcache-v1-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/caamtech/refs/heads/main/openapi/caamtech-objectcache-v1-api-openapi.yml
- filename: caamtech-oembed-1-0-api-openapi.yml
  format: yaml
  label: CaaMTech Oembed/1.0 API
  slug: caamtech-oembed-1-0-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/caamtech/refs/heads/main/openapi/caamtech-oembed-1-0-api-openapi.yml
- filename: caamtech-regenerate-thumbnails-v1-api-openapi.yml
  format: yaml
  label: CaaMTech Regenerate Thumbnails/v1 API
  slug: caamtech-regenerate-thumbnails-v1-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/caamtech/refs/heads/main/openapi/caamtech-regenerate-thumbnails-v1-api-openapi.yml
- filename: caamtech-root-api-openapi.yml
  format: yaml
  label: CaaMTech Root API
  slug: caamtech-root-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/caamtech/refs/heads/main/openapi/caamtech-root-api-openapi.yml
- filename: caamtech-wp-abilities-v1-api-openapi.yml
  format: yaml
  label: CaaMTech Wp Abilities/v1 API
  slug: caamtech-wp-abilities-v1-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/caamtech/refs/heads/main/openapi/caamtech-wp-abilities-v1-api-openapi.yml
- filename: caamtech-wp-block-editor-v1-api-openapi.yml
  format: yaml
  label: CaaMTech Wp Block Editor/v1 API
  slug: caamtech-wp-block-editor-v1-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/caamtech/refs/heads/main/openapi/caamtech-wp-block-editor-v1-api-openapi.yml
- filename: caamtech-wp-site-health-v1-api-openapi.yml
  format: yaml
  label: CaaMTech Wp Site Health/v1 API
  slug: caamtech-wp-site-health-v1-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/caamtech/refs/heads/main/openapi/caamtech-wp-site-health-v1-api-openapi.yml
- filename: caamtech-wp-v2-api-openapi.yml
  format: yaml
  label: CaaMTech Wp/v2 API
  slug: caamtech-wp-v2-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/caamtech/refs/heads/main/openapi/caamtech-wp-v2-api-openapi.yml
- filename: caamtech-wpforms-v1-api-openapi.yml
  format: yaml
  label: CaaMTech Wpforms/v1 API
  slug: caamtech-wpforms-v1-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/caamtech/refs/heads/main/openapi/caamtech-wpforms-v1-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: probed
name: Caamtech Authentication
name_suffix: Authentication
oauth_flows: []
overview: CaaMTech secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: CaaMTech
provider_slug: caamtech
scheme_count: 2
schemes:
- description: WordPress Application Passwords (HTTP Basic). The site advertises the authorization endpoint at https://caam.tech/wp-admin/authorize-application.php
  name: applicationPassword
  scheme: basic
  sources:
  - openapi/caamtech-wordpress-rest-openapi.yml
  type: http
- description: WordPress logged-in cookie plus an X-WP-Nonce header (first-party only).
  in: cookie
  name: cookieAuth
  parameter: wordpress_logged_in
  sources:
  - openapi/caamtech-wordpress-rest-openapi.yml
  type: apiKey
slug: caamtech-authentication
source_filename: caamtech-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-08'\nmethod: probed\nsource: https://caam.tech/wp-json/\nderived_from: openapi/caamtech-wordpress-rest-openapi.yml\nnotes: >-\n  CaaMTech publishes no developer authentication documentation. The auth model below is the\n  one the site's own WordPress REST discovery document advertises. Anonymous GET requests to\n  the read-only content routes succeed without any credential; every write route and the MCP\n  adapter route require a WordPress credential.\nauthorization_endpoint: https://caam.tech/wp-admin/authorize-application.php\nx-evidence:\n- fetched: '2026-08-08'\n  url: https://caam.tech/wp-json/\n  http_status: 200\n  finding: >-\n    `authentication` block advertises application-passwords with the authorization endpoint\n    https://caam.tech/wp-admin/authorize-application.php\n- fetched: '2026-08-08'\n  url: https://caam.tech/wp-json/wp/v2/posts?per_page=1\n  http_status: 200\n  finding: anonymous read succeeds with no credential\n- fetched: '2026-08-08'\n\
  \  url: https://caam.tech/wp-json/mcp/mcp-adapter-default-server\n  http_status: 401\n  finding: 'MCP tools/list returns {\"code\":\"rest_forbidden\",\"data\":{\"status\":401}}'\nanonymous_read: true\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - cookie\nschemes:\n- name: applicationPassword\n  type: http\n  scheme: basic\n  description: WordPress Application Passwords (HTTP Basic). The site advertises the authorization\n    endpoint at https://caam.tech/wp-admin/authorize-application.php\n  sources:\n  - openapi/caamtech-wordpress-rest-openapi.yml\n- name: cookieAuth\n  type: apiKey\n  in: cookie\n  parameter: wordpress_logged_in\n  description: WordPress logged-in cookie plus an X-WP-Nonce header (first-party only).\n  sources:\n  - openapi/caamtech-wordpress-rest-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/caamtech/refs/heads/main/authentication/caamtech-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Company
- Pharmaceuticals
- Life Sciences
- Drug Discovery
- Biotechnology
- Chemistry
- Mental Health
- Research
- Psychedelics
- WordPress
---
