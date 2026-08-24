---
api_key_in: []
api_specs:
- filename: impossible-metals-posts-openapi.yml
  format: yaml
  label: Impossible Metals Posts API
  slug: impossible-metals-posts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/impossible-metals/refs/heads/main/openapi/impossible-metals-posts-openapi.yml
- filename: impossible-metals-pages-openapi.yml
  format: yaml
  label: Impossible Metals Pages API
  slug: impossible-metals-pages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/impossible-metals/refs/heads/main/openapi/impossible-metals-pages-openapi.yml
- filename: impossible-metals-faq-openapi.yml
  format: yaml
  label: Impossible Metals FAQ API
  slug: impossible-metals-faq-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/impossible-metals/refs/heads/main/openapi/impossible-metals-faq-openapi.yml
- filename: impossible-metals-media-openapi.yml
  format: yaml
  label: Impossible Metals Media API
  slug: impossible-metals-media-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/impossible-metals/refs/heads/main/openapi/impossible-metals-media-openapi.yml
- filename: impossible-metals-taxonomy-openapi.yml
  format: yaml
  label: Impossible Metals Taxonomy API
  slug: impossible-metals-taxonomy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/impossible-metals/refs/heads/main/openapi/impossible-metals-taxonomy-openapi.yml
- filename: impossible-metals-search-openapi.yml
  format: yaml
  label: Impossible Metals Search API
  slug: impossible-metals-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/impossible-metals/refs/heads/main/openapi/impossible-metals-search-openapi.yml
- filename: impossible-metals-events-openapi.yml
  format: yaml
  label: Impossible Metals Events API
  slug: impossible-metals-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/impossible-metals/refs/heads/main/openapi/impossible-metals-events-openapi.yml
- filename: impossible-metals-events-tec-openapi.yml
  format: yaml
  label: Impossible Metals Events API (TEC v1, experimental)
  slug: impossible-metals-events-tec-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/impossible-metals/refs/heads/main/openapi/impossible-metals-events-tec-openapi.yml
- filename: impossible-metals-discovery-openapi.yml
  format: yaml
  label: Impossible Metals Discovery API
  slug: impossible-metals-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/impossible-metals/refs/heads/main/openapi/impossible-metals-discovery-openapi.yml
- filename: impossible-metals-oembed-openapi.yml
  format: yaml
  label: Impossible Metals oEmbed API
  slug: impossible-metals-oembed-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/impossible-metals/refs/heads/main/openapi/impossible-metals-oembed-openapi.yml
auth_types:
- none
- http
description: ''
kind: authentication
layout: security
method: derived
name: Impossible Metals Authentication
name_suffix: Authentication
oauth_flows: []
overview: Impossible Metals secures its APIs with none and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Impossible Metals
provider_slug: impossible-metals
scheme_count: 2
schemes:
- description: Anonymous read. GET on /wp-json/wp/v2/posts, /pages, /media, /avada_faq, /faq_category, /categories, /tags, /types, /taxonomies, /users, /statuses, /search, on /wp-json/oembed/1.0/embed and on /wp-json/tribe/events/v1/* all returned 200 without credentials. This is the surface an agent can actually call.
  name: none
  sources:
  - live probe 2026-08-23
  type: none
- authorization_endpoint: https://impossiblemetals.com/wp-admin/authorize-application.php
  description: WordPress Application Passwords over HTTP Basic. The route index advertises this as the site's only supported authentication mechanism, with the authorization endpoint at https://impossiblemetals.com/wp-admin/authorize-application.php. It gates the write half of the content routes (POST/PUT/DELETE) and the administrative routes. It is issued per WordPress user from the admin console — it is a site-administrator credential, not a developer credential, and Impossible Metals publishes no process for a third party to obtain one.
  name: ApplicationPasswords
  scheme: basic
  sources:
  - https://impossiblemetals.com/wp-json/ (authentication.application-passwords)
  - openapi/impossible-metals-events-tec-openapi.yml (components.securitySchemes.BasicAuth)
  type: http
slug: impossible-metals-authentication
source_filename: impossible-metals-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-23'\nmethod: derived\nsource: >-\n  https://impossiblemetals.com/wp-json/ (the site's own route index, which advertises the supported\n  authentication mechanism) + openapi/impossible-metals-events-tec-openapi.yml (the published\n  securitySchemes block) + live anonymous probes of every collection route on 2026-08-23.\nsummary:\n  types:\n  - none\n  - http\n  anonymous_read: true\n  note: >-\n    The entire public surface profiled in this repo is anonymously readable. Every collection route\n    answered HTTP 200 with `Allow: GET` and no credentials on 2026-08-23. There is no API key, no\n    OAuth, no OpenID Connect and no signup — because there is no developer program. Authentication\n    only appears on the write half of the same routes, which is not part of the public surface.\nschemes:\n- name: none\n  type: none\n  description: >-\n    Anonymous read. GET on /wp-json/wp/v2/posts, /pages, /media, /avada_faq, /faq_category,\n    /categories, /tags,\
  \ /types, /taxonomies, /users, /statuses, /search, on /wp-json/oembed/1.0/embed\n    and on /wp-json/tribe/events/v1/* all returned 200 without credentials. This is the surface an\n    agent can actually call.\n  sources:\n  - live probe 2026-08-23\n- name: ApplicationPasswords\n  type: http\n  scheme: basic\n  description: >-\n    WordPress Application Passwords over HTTP Basic. The route index advertises this as the site's\n    only supported authentication mechanism, with the authorization endpoint at\n    https://impossiblemetals.com/wp-admin/authorize-application.php. It gates the write half of the\n    content routes (POST/PUT/DELETE) and the administrative routes. It is issued per WordPress user\n    from the admin console — it is a site-administrator credential, not a developer credential, and\n    Impossible Metals publishes no process for a third party to obtain one.\n  authorization_endpoint: https://impossiblemetals.com/wp-admin/authorize-application.php\n  sources:\n  - https://impossiblemetals.com/wp-json/\
  \ (authentication.application-passwords)\n  - openapi/impossible-metals-events-tec-openapi.yml (components.securitySchemes.BasicAuth)\ngated_routes:\n- route: /wp-json/wp/v2/settings\n  status: 401\n  note: Returns 401 rest_forbidden_context anonymously.\n- route: /wp-json/wp/v2/block-types\n  status: 401\n  note: Returns 401 anonymously.\n- route: /wp-json/tec/v1/*\n  status: 400\n  note: >-\n    Not an authentication gate. Returns 400 missing_experimental_endpoint_acknowledgement — the TEC\n    v1 routes are flagged experimental and require an acknowledgement header before they will answer,\n    authenticated or not.\noauth: false\nopenid_connect: false\nmutual_tls: false\napi_keys: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/impossible-metals/refs/heads/main/authentication/impossible-metals-authentication.yml
summary_line: none/http · 2 schemes
tags:
- Company
- Deep Sea Mining
- Critical Minerals
- Battery Metals
- Robotics
- Autonomous Underwater Vehicles
- Ocean Technology
- Mining
- Sustainability
- Climate Tech
- Content
- Events
---
