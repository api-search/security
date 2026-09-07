---
anonymous_access: false
api_key_in: []
api_specs:
- filename: endeavor-content-api-openapi.yml
  format: yaml
  label: WME Group Content API (WordPress REST wp/v2)
  slug: content-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/endeavor/refs/heads/main/openapi/endeavor-content-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Endeavor Authentication
name_suffix: Authentication
oauth_flows: []
overview: Endeavor secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Endeavor
provider_slug: endeavor
scheme_count: 1
schemes:
- description: WordPress Application Passwords over HTTP Basic. Issued from /wp-admin/authorize-application.php by an authenticated site user; not available to the public.
  name: applicationPassword
  scheme: basic
  sources:
  - openapi/endeavor-content-api-openapi.yml
  type: http
slug: endeavor-authentication
source_filename: endeavor-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-06'\nmethod: derived\nsource: openapi/endeavor-content-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: applicationPassword\n  type: http\n  scheme: basic\n  description: WordPress Application Passwords over HTTP Basic. Issued from /wp-admin/authorize-application.php\n    by an authenticated site user; not available to the public.\n  sources:\n  - openapi/endeavor-content-api-openapi.yml\nanonymous_read:\n  supported: true\n  note: >-\n    The public content collections of the wmegrp.com WordPress REST API are readable with NO\n    credentials at all — /wp/v2/posts, /wp/v2/pages, /wp/v2/media, /wp/v2/categories, /wp/v2/tags,\n    /wp/v2/search, /wp/v2/types, /wp/v2/taxonomies and /wp/v2/statuses all returned HTTP 200 to an\n    unauthenticated GET on 2026-09-06. Administrative collections (/wp/v2/users, /wp/v2/settings,\n    /wp/v2/themes, /wp/v2/plugins, /wp/v2/menus, /wp/v2/widgets, /wp/v2/templates) returned HTTP 401.\n  verified: probed\n\
  \  checked: '2026-09-06'\ngated_surfaces:\n- url: https://wmegrp.com/wp-json/mcp/mcp-adapter-default-server\n  status: 401\n  code: rest_forbidden\n- url: https://wmegrp.com/wp-json/wp-abilities/v1/abilities\n  status: 401\n  code: rest_forbidden\noauth:\n  published: false\n  discovery:\n  - url: https://wmegrp.com/.well-known/oauth-authorization-server\n    status: 404\n  - url: https://wmegrp.com/.well-known/openid-configuration\n    status: 404\nnote: >-\n  Endeavor / WME Group publishes no authentication documentation. Everything here is derived from the\n  mechanically-derived OpenAPI plus live anonymous probes; the scheme is WordPress core behaviour, not\n  a documented company policy.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/endeavor/refs/heads/main/authentication/endeavor-authentication.yml
summary_line: http · 1 scheme
tags:
- Sports
- Entertainment
- Talent
- Media
- Licensing
- Marketing
---
