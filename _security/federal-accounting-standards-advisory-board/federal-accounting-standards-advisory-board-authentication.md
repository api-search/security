---
anonymous_access: true
api_key_in: []
api_specs:
- filename: federal-accounting-standards-advisory-board-wp-content-openapi.yml
  format: yaml
  label: FASAB Public Content API (WordPress REST)
  slug: federal-accounting-standards-advisory-board-wp-content
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/federal-accounting-standards-advisory-board/refs/heads/main/openapi/federal-accounting-standards-advisory-board-wp-content-openapi.yml
auth_types:
- none
- basic
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: probed
name: Federal Accounting Standards Advisory Board Authentication
name_suffix: Authentication
oauth_flows: []
overview: Federal Accounting Standards Advisory Board secures its APIs with none and basic across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Federal Accounting Standards Advisory Board
provider_slug: federal-accounting-standards-advisory-board
scheme_count: 2
schemes:
- description: 'The public read surface. No Authorization header, API key, cookie or nonce is required; the `security: [{}]` block in the derived OpenAPI reflects the observed behaviour. Verified against /wp/v2/posts, /wp/v2/pages, /wp/v2/media, /wp/v2/search, /wp/v2/types, /wp/v2/taxonomies and the route index on 2026-09-09.'
  evidence:
  - anonymous: true
    http_status: 200
    url: https://fasab.gov/wp-json/wp/v2/pages?per_page=1
  name: anonymous
  sources:
  - openapi/federal-accounting-standards-advisory-board-wp-content-openapi.yml
  type: none
- authorization_endpoint: https://fasab.gov/wp-admin/authorize-application.php
  description: WordPress Application Passwords, declared by fasab.gov itself in the `authentication` object of its REST discovery document. Credentials are HTTP Basic (WordPress username + a generated application password) and are issued interactively from wp-admin. This governs the AUTHENTICATED surface only — the administrative and plugin namespaces that answer 401 rest_forbidden anonymously — and is available to FASAB site operators, not to the public. There is no self-service registration.
  evidence:
  - field: authentication['application-passwords'].endpoints.authorization
    http_status: 200
    url: https://fasab.gov/wp-json/
  name: application-passwords
  scheme: basic
  sources:
  - https://fasab.gov/wp-json/
  type: http
slug: federal-accounting-standards-advisory-board-authentication
source_filename: federal-accounting-standards-advisory-board-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-09'\nmethod: probed\nsource: https://fasab.gov/wp-json/\ndocs: null\nnote: >-\n  FASAB publishes no authentication documentation. This profile records what the site's own WordPress\n  REST discovery document declares and what unauthenticated requests actually observed on 2026-09-09.\n  The public read surface requires NO credential at all — every one of the 28 operations in\n  openapi/federal-accounting-standards-advisory-board-wp-content-openapi.yml returned HTTP 200 anonymously.\nsummary:\n  types:\n  - none\n  - basic\n  api_key_in: []\n  oauth2_flows: []\n  public_read: true\nschemes:\n- name: anonymous\n  type: none\n  description: >-\n    The public read surface. No Authorization header, API key, cookie or nonce is required; the\n    `security: [{}]` block in the derived OpenAPI reflects the observed behaviour. Verified against\n    /wp/v2/posts, /wp/v2/pages, /wp/v2/media, /wp/v2/search, /wp/v2/types, /wp/v2/taxonomies and the\n    route index on\
  \ 2026-09-09.\n  sources:\n  - openapi/federal-accounting-standards-advisory-board-wp-content-openapi.yml\n  evidence:\n  - url: https://fasab.gov/wp-json/wp/v2/pages?per_page=1\n    http_status: 200\n    anonymous: true\n- name: application-passwords\n  type: http\n  scheme: basic\n  description: >-\n    WordPress Application Passwords, declared by fasab.gov itself in the `authentication` object of its\n    REST discovery document. Credentials are HTTP Basic (WordPress username + a generated application\n    password) and are issued interactively from wp-admin. This governs the AUTHENTICATED surface only —\n    the administrative and plugin namespaces that answer 401 rest_forbidden anonymously — and is\n    available to FASAB site operators, not to the public. There is no self-service registration.\n  authorization_endpoint: https://fasab.gov/wp-admin/authorize-application.php\n  sources:\n  - https://fasab.gov/wp-json/\n  evidence:\n  - url: https://fasab.gov/wp-json/\n    http_status:\
  \ 200\n    field: authentication['application-passwords'].endpoints.authorization\ngated_surface:\n  note: Routes confirmed to require authentication (HTTP 401 rest_forbidden anonymously, 2026-09-09).\n  probes:\n  - {url: 'https://fasab.gov/wp-json/wp/v2/settings', http_status: 401}\n  - {url: 'https://fasab.gov/wp-json/wp/v2/plugins', http_status: 401}\n  - {url: 'https://fasab.gov/wp-json/wp/v2/themes', http_status: 401}\n  - {url: 'https://fasab.gov/wp-json/wp/v2/block-types', http_status: 401}\n  - {url: 'https://fasab.gov/wp-json/wp/v2/users/me', http_status: 401}\n  - {url: 'https://fasab.gov/wp-json/wp/v2/posts/12417/revisions', http_status: 401}\n  - {url: 'https://fasab.gov/wp-json/wp-abilities/v1/abilities', http_status: 401}\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/federal-accounting-standards-advisory-board/refs/heads/main/authentication/federal-accounting-standards-advisory-board-authentication.yml
summary_line: none/basic · 2 schemes
tags:
- Accounting
- Federal-Government
- Standards
- Financial-Reporting
- Government
- Regulations
- Content
- Publications
---
