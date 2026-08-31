---
api_key_in: []
api_specs:
- filename: ksq-therapeutics-pages-api-openapi.yml
  format: yaml
  label: KSQ Therapeutics Pages API
  slug: ksq-therapeutics-pages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ksq-therapeutics/refs/heads/main/openapi/ksq-therapeutics-pages-api-openapi.yml
- filename: ksq-therapeutics-media-api-openapi.yml
  format: yaml
  label: KSQ Therapeutics Media API
  slug: ksq-therapeutics-media-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ksq-therapeutics/refs/heads/main/openapi/ksq-therapeutics-media-api-openapi.yml
- filename: ksq-therapeutics-search-api-openapi.yml
  format: yaml
  label: KSQ Therapeutics Search API
  slug: ksq-therapeutics-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ksq-therapeutics/refs/heads/main/openapi/ksq-therapeutics-search-api-openapi.yml
- filename: ksq-therapeutics-discovery-api-openapi.yml
  format: yaml
  label: KSQ Therapeutics Discovery API
  slug: ksq-therapeutics-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ksq-therapeutics/refs/heads/main/openapi/ksq-therapeutics-discovery-api-openapi.yml
- filename: ksq-therapeutics-taxonomy-api-openapi.yml
  format: yaml
  label: KSQ Therapeutics Taxonomy API
  slug: ksq-therapeutics-taxonomy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ksq-therapeutics/refs/heads/main/openapi/ksq-therapeutics-taxonomy-api-openapi.yml
- filename: ksq-therapeutics-posts-api-openapi.yml
  format: yaml
  label: KSQ Therapeutics Posts API
  slug: ksq-therapeutics-posts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ksq-therapeutics/refs/heads/main/openapi/ksq-therapeutics-posts-api-openapi.yml
- filename: ksq-therapeutics-oembed-api-openapi.yml
  format: yaml
  label: KSQ Therapeutics oEmbed API
  slug: ksq-therapeutics-oembed-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ksq-therapeutics/refs/heads/main/openapi/ksq-therapeutics-oembed-api-openapi.yml
- filename: ksq-therapeutics-press-release-api-openapi.yml
  format: yaml
  label: KSQ Therapeutics Press Release API
  slug: ksq-therapeutics-press-release-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ksq-therapeutics/refs/heads/main/openapi/ksq-therapeutics-press-release-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
method: derived
name: Ksq Therapeutics Authentication
name_suffix: Authentication
oauth_flows: []
overview: KSQ Therapeutics declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: KSQ Therapeutics
provider_slug: ksq-therapeutics
scheme_count: 2
schemes:
- applies_to: read
  description: 'Every operation catalogued in openapi/ is anonymously readable. Verified on 2026-08-23 with no Authorization header: /wp/v2/pages, /wp/v2/media, /wp/v2/press_release, /wp/v2/posts, /wp/v2/search, /wp/v2/categories, /wp/v2/tags, /wp/v2/types, /wp/v2/taxonomies, /wp/v2/statuses, /oembed/1.0/embed and the route index at / all returned HTTP 200.'
  id: anonymous
  type: none
- applies_to: write, administrative
  authorization_url: https://ksqtx.com/wp-admin/authorize-application.php
  description: WordPress Application Passwords, declared verbatim in the site's own route index under authentication["application-passwords"]. Credentials are issued per-user from https://ksqtx.com/wp-admin/authorize-application.php and presented as HTTP Basic. This is the only authentication mechanism the deployment advertises. It gates writes and the administrative namespaces; there is no self-service path to obtain one, and API Evangelist holds none.
  id: application-passwords
  scheme: basic
  type: http
  x-evidence:
    field: authentication.application-passwords.endpoints.authorization
    http_status: 200
    url: https://ksqtx.com/wp-json/
slug: ksq-therapeutics-authentication
source_filename: ksq-therapeutics-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-23'\nmethod: derived\nsource: >-\n  openapi/_original/ksq-therapeutics-content-openapi.yml plus live anonymous probes of\n  https://ksqtx.com/wp-json/ on 2026-08-23. The authentication block of the WordPress REST route\n  index at https://ksqtx.com/wp-json/ was read verbatim.\nnote: >-\n  KSQ Therapeutics publishes no developer authentication documentation, no OAuth server, no API key\n  programme and no signup flow, because it publishes no product API. What is described here is the\n  authentication model of the WordPress REST API running its corporate marketing site. The read\n  surface catalogued in this repo requires no credentials at all; everything that would require one\n  is administrative.\napi: https://ksqtx.com/wp-json\nschemes:\n- id: anonymous\n  type: none\n  description: >-\n    Every operation catalogued in openapi/ is anonymously readable. Verified on 2026-08-23 with no\n    Authorization header: /wp/v2/pages, /wp/v2/media, /wp/v2/press_release,\
  \ /wp/v2/posts,\n    /wp/v2/search, /wp/v2/categories, /wp/v2/tags, /wp/v2/types, /wp/v2/taxonomies, /wp/v2/statuses,\n    /oembed/1.0/embed and the route index at / all returned HTTP 200.\n  applies_to: read\n- id: application-passwords\n  type: http\n  scheme: basic\n  description: >-\n    WordPress Application Passwords, declared verbatim in the site's own route index under\n    authentication[\"application-passwords\"]. Credentials are issued per-user from\n    https://ksqtx.com/wp-admin/authorize-application.php and presented as HTTP Basic. This is the\n    only authentication mechanism the deployment advertises. It gates writes and the administrative\n    namespaces; there is no self-service path to obtain one, and API Evangelist holds none.\n  authorization_url: https://ksqtx.com/wp-admin/authorize-application.php\n  applies_to: write, administrative\n  x-evidence:\n    url: https://ksqtx.com/wp-json/\n    field: authentication.application-passwords.endpoints.authorization\n   \
  \ http_status: 200\noauth2: false\nopenid_connect: false\nmutual_tls: false\napi_keys: false\ngated_surfaces:\n- path: /wp/v2/settings\n  status: 401\n  code: rest_forbidden\n- path: /wp/v2/users/me\n  status: 401\n  code: rest_forbidden\n- path: /wp-abilities/v1/abilities\n  status: 401\n  code: rest_forbidden\n- path: /aioseo/v1/ping\n  status: 401\n  code: rest_forbidden\n- path: /aioseo/v1/options\n  status: 401\n  code: rest_forbidden\n- path: /cky/v1/settings/info\n  status: 401\n  code: cookieyes_rest_cannot_view\n- path: /redirection/v1/redirect\n  status: 401\n  code: rest_forbidden\nobservations:\n- >-\n  /wp/v2/users returned HTTP 200 anonymously with 3 author records on 2026-08-23. This is the\n  WordPress default author-enumeration surface, not a KSQ decision. The identities are not recorded\n  in this repo.\n- >-\n  context=edit is refused anonymously on every collection; only context=view and context=embed are\n  reachable without credentials.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ksq-therapeutics/refs/heads/main/authentication/ksq-therapeutics-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Biotechnology
- Life Sciences
- Therapeutics
- Oncology
- Genomics
- CRISPR
- Gene Editing
- Cell Therapy
- Clinical Stage
- Functional Genomics
- content-api
---
