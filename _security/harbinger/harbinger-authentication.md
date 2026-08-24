---
api_key_in: []
api_specs:
- filename: harbinger-posts-api-openapi.yml
  format: yaml
  label: Harbinger Motors Posts API
  slug: harbinger-posts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/harbinger/refs/heads/main/openapi/harbinger-posts-api-openapi.yml
- filename: harbinger-pages-api-openapi.yml
  format: yaml
  label: Harbinger Motors Pages API
  slug: harbinger-pages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/harbinger/refs/heads/main/openapi/harbinger-pages-api-openapi.yml
- filename: harbinger-events-api-openapi.yml
  format: yaml
  label: Harbinger Motors Events API
  slug: harbinger-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/harbinger/refs/heads/main/openapi/harbinger-events-api-openapi.yml
- filename: harbinger-media-api-openapi.yml
  format: yaml
  label: Harbinger Motors Media API
  slug: harbinger-media-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/harbinger/refs/heads/main/openapi/harbinger-media-api-openapi.yml
- filename: harbinger-taxonomy-api-openapi.yml
  format: yaml
  label: Harbinger Motors Taxonomy API
  slug: harbinger-taxonomy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/harbinger/refs/heads/main/openapi/harbinger-taxonomy-api-openapi.yml
- filename: harbinger-search-api-openapi.yml
  format: yaml
  label: Harbinger Motors Search API
  slug: harbinger-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/harbinger/refs/heads/main/openapi/harbinger-search-api-openapi.yml
- filename: harbinger-discovery-api-openapi.yml
  format: yaml
  label: Harbinger Motors Discovery API
  slug: harbinger-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/harbinger/refs/heads/main/openapi/harbinger-discovery-api-openapi.yml
- filename: harbinger-oembed-api-openapi.yml
  format: yaml
  label: Harbinger Motors oEmbed API
  slug: harbinger-oembed-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/harbinger/refs/heads/main/openapi/harbinger-oembed-api-openapi.yml
- filename: harbinger-seo-api-openapi.yml
  format: yaml
  label: Harbinger Motors SEO Metadata API
  slug: harbinger-seo-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/harbinger/refs/heads/main/openapi/harbinger-seo-api-openapi.yml
auth_types: []
description: Harbinger Motors publishes no developer program, no API key issuance, no OAuth application registration and no authentication documentation. The WordPress REST content API behind harbingermotors.com is anonymously readable and, anonymously, read-only. Everything below was observed on live responses on 2026-08-22.
kind: authentication
layout: security
method: probed
name: Harbinger Authentication
name_suffix: Authentication
oauth_flows: []
overview: Harbinger declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: Harbinger
provider_slug: harbinger
scheme_count: 0
schemes: []
slug: harbinger-authentication
source_filename: harbinger-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-22'\nmethod: probed\nsource: live probes of https://harbingermotors.com/wp-json/ + the route index it publishes\ndescription: >-\n  Harbinger Motors publishes no developer program, no API key issuance, no OAuth application\n  registration and no authentication documentation. The WordPress REST content API behind\n  harbingermotors.com is anonymously readable and, anonymously, read-only. Everything below was\n  observed on live responses on 2026-08-22.\npublic_read: true\nschemes: []\ndeclared_security_schemes: 0\nanonymous_access:\n  supported: true\n  detail: >-\n    Every operation captured in openapi/ answers 200 with no credential of any kind. The collection\n    routes return `Allow: GET` to an anonymous OPTIONS, which is the server itself stating that GET\n    is the only method available without authentication.\n  evidence:\n  - url: https://harbingermotors.com/wp-json/wp/v2/posts?per_page=2\n    http_status: 200\n    header: 'allow: GET'\nwrite_access:\n\
  \  supported_anonymously: false\n  mechanism: WordPress application passwords (HTTP Basic over TLS) or a logged-in session nonce\n  public_issuance_path: none\n  detail: >-\n    The same routes register POST/PUT/PATCH/DELETE endpoints, but they are capability-gated. An\n    anonymous POST to /wp/v2/posts returns 401 rest_cannot_create. Application passwords can only\n    be minted from inside the WordPress admin by an account Harbinger controls, so there is no path\n    for a third party to obtain write credentials. Treat this surface as read-only.\n  evidence:\n  - url: https://harbingermotors.com/wp-json/wp/v2/posts\n    method: POST\n    http_status: 401\n    code: rest_cannot_create\nadvertised_schemes:\n  detail: >-\n    The API index publishes an `authentication` key and it is an empty array on this host — the\n    server advertises no authentication scheme at all. Application-password support is present in\n    core (the /wp/v2/users/{id}/application-passwords routes are registered)\
  \ but is not advertised\n    as a public scheme.\n  evidence:\n  - url: https://harbingermotors.com/wp-json/\n    http_status: 200\n    observed: 'authentication: []'\ngated_routes_observed:\n- {route: /wp/v2/users, status: 401, code: rest_user_cannot_view}\n- {route: /wp/v2/settings, status: 401, code: rest_forbidden}\n- {route: /wp/v2/menus, status: 401, code: rest_cannot_view}\n- {route: /wp/v2/block-types, status: 401, code: rest_block_type_cannot_view}\n- {route: /wp-abilities/v1/abilities, status: 401, code: rest_forbidden}\n- {route: '/wp/v2/posts?context=edit', status: 401, code: rest_forbidden_context}\ntransport:\n  tls: true\n  tls_version: TLSv1.3\n  hsts: false\n  note: >-\n    HTTPS is enforced by redirect but no Strict-Transport-Security header is returned, so a first\n    request to http:// is not protected by HSTS preloading. See security/harbinger-domain-security.yml.\nnote: >-\n  No scopes/ artifact is emitted: there is no OAuth surface here, so a scope file would be\
  \ an empty\n  artifact rather than a finding.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/harbinger/refs/heads/main/authentication/harbinger-authentication.yml
summary_line: 0 schemes
tags:
- Company
- Automotive
- Electric Vehicles
- Commercial Vehicles
- Medium Duty Trucks
- Manufacturing
- Fleet Management
- Transportation
- Logistics
- Energy Storage
- Content
---
