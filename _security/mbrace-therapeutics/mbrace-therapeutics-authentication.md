---
api_key_in: []
api_specs:
- filename: mbrace-therapeutics-news-openapi.yml
  format: yaml
  label: MBrace Therapeutics News API
  slug: mbrace-therapeutics-news-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mbrace-therapeutics/refs/heads/main/openapi/mbrace-therapeutics-news-openapi.yml
- filename: mbrace-therapeutics-people-openapi.yml
  format: yaml
  label: MBrace Therapeutics People API
  slug: mbrace-therapeutics-people-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mbrace-therapeutics/refs/heads/main/openapi/mbrace-therapeutics-people-openapi.yml
- filename: mbrace-therapeutics-pages-openapi.yml
  format: yaml
  label: MBrace Therapeutics Pages API
  slug: mbrace-therapeutics-pages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mbrace-therapeutics/refs/heads/main/openapi/mbrace-therapeutics-pages-openapi.yml
- filename: mbrace-therapeutics-media-openapi.yml
  format: yaml
  label: MBrace Therapeutics Media API
  slug: mbrace-therapeutics-media-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mbrace-therapeutics/refs/heads/main/openapi/mbrace-therapeutics-media-openapi.yml
- filename: mbrace-therapeutics-taxonomy-openapi.yml
  format: yaml
  label: MBrace Therapeutics Taxonomy API
  slug: mbrace-therapeutics-taxonomy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mbrace-therapeutics/refs/heads/main/openapi/mbrace-therapeutics-taxonomy-openapi.yml
- filename: mbrace-therapeutics-search-openapi.yml
  format: yaml
  label: MBrace Therapeutics Search API
  slug: mbrace-therapeutics-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mbrace-therapeutics/refs/heads/main/openapi/mbrace-therapeutics-search-openapi.yml
- filename: mbrace-therapeutics-discovery-openapi.yml
  format: yaml
  label: MBrace Therapeutics Discovery API
  slug: mbrace-therapeutics-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mbrace-therapeutics/refs/heads/main/openapi/mbrace-therapeutics-discovery-openapi.yml
- filename: mbrace-therapeutics-users-openapi.yml
  format: yaml
  label: MBrace Therapeutics Users API
  slug: mbrace-therapeutics-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mbrace-therapeutics/refs/heads/main/openapi/mbrace-therapeutics-users-openapi.yml
- filename: mbrace-therapeutics-oembed-openapi.yml
  format: yaml
  label: MBrace Therapeutics oEmbed API
  slug: mbrace-therapeutics-oembed-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mbrace-therapeutics/refs/heads/main/openapi/mbrace-therapeutics-oembed-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
method: probed
name: Mbrace Therapeutics Authentication
name_suffix: Authentication
oauth_flows: []
overview: MBrace Therapeutics declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: MBrace Therapeutics
provider_slug: mbrace-therapeutics
scheme_count: 2
schemes:
- applies_to: Every operation in openapi/ — the news, people, pages, media, taxonomy, search, discovery, users and oEmbed surfaces.
  detail: 'Verified live on 2026-08-25: GET https://mbracetrx.com/wp-json/wp/v2/posts returned 200 with no Authorization header, no cookie and no nonce.'
  id: none
  type: none
- advertised_at: https://mbracetrx.com/wp-json/
  applies_to: The write surface and the authenticated administration namespaces. NOT catalogued in openapi/ — they were confirmed gated and were never exercised.
  authorization_endpoint: https://mbracetrx.com/wp-admin/authorize-application.php
  detail: The discovery document advertises `authentication.application-passwords.endpoints.authorization`. This is WordPress core's per-user application-password mechanism, sent as HTTP Basic. It is issued from inside wp-admin by an already-authenticated user; there is no public registration, no key management page and no documented scope model. It is not an API product.
  id: application-passwords
  scheme: basic
  self_service: false
  type: http
slug: mbrace-therapeutics-authentication
source_filename: mbrace-therapeutics-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-25'\nmethod: probed\nsource: https://mbracetrx.com/wp-json/ (authentication block + live anonymous responses, 2026-08-25)\nnote: >-\n  MBrace Therapeutics publishes no authentication documentation of its own — there is no developer\n  portal and no API reference. Everything below was read from the live deployment: the\n  `authentication` block of the WordPress REST discovery document, and the actual status codes\n  returned to unauthenticated requests. The derive-authentication.py pass produced no profile because\n  none of the harvested OpenAPI documents declare a `securitySchemes` block, and that is correct\n  rather than a gap: every operation catalogued in openapi/ is anonymously readable and requires no\n  credential at all.\nsummary:\n  anonymous_read: true\n  credential_required_for_catalogued_operations: false\n  schemes_advertised:\n  - application-passwords\n  detail: >-\n    All 28 catalogued operations are anonymous GETs. No API key, no bearer\
  \ token, no OAuth, no\n    mutual TLS. The only credential scheme the deployment advertises is WordPress application\n    passwords, which is an administrative credential for the WordPress backend, not a consumer API\n    credential — it cannot be self-issued and there is no signup flow for it.\nschemes:\n- id: none\n  type: none\n  applies_to: >-\n    Every operation in openapi/ — the news, people, pages, media, taxonomy, search, discovery, users\n    and oEmbed surfaces.\n  detail: >-\n    Verified live on 2026-08-25: GET https://mbracetrx.com/wp-json/wp/v2/posts returned 200 with no\n    Authorization header, no cookie and no nonce.\n- id: application-passwords\n  type: http\n  scheme: basic\n  advertised_at: https://mbracetrx.com/wp-json/\n  authorization_endpoint: https://mbracetrx.com/wp-admin/authorize-application.php\n  applies_to: >-\n    The write surface and the authenticated administration namespaces. NOT catalogued in openapi/ —\n    they were confirmed gated and were never\
  \ exercised.\n  self_service: false\n  detail: >-\n    The discovery document advertises `authentication.application-passwords.endpoints.authorization`.\n    This is WordPress core's per-user application-password mechanism, sent as HTTP Basic. It is\n    issued from inside wp-admin by an already-authenticated user; there is no public registration,\n    no key management page and no documented scope model. It is not an API product.\ngated_surfaces_observed:\n- path: /wp-json/wp/v2/settings\n  status: 401\n  code: rest_forbidden\n- path: /wp-json/wp/v2/menus\n  status: 401\n  code: rest_cannot_view\n- path: /wp-json/wp/v2/plugins\n  status: 401\n  code: rest_cannot_view_plugins\n- path: /wp-json/wp/v2/themes\n  status: 401\n  code: rest_cannot_view_themes\n- path: /wp-json/wp-abilities/v1/abilities\n  status: 401\n  code: rest_forbidden\n  detail: >-\n    The WordPress Abilities API namespace is registered on this deployment but returns 401\n    anonymously. See mcp/mbrace-therapeutics-mcp.yml\
  \ — this is the closest thing to an agent-tool\n    surface here, and it is not open.\n- path: /wp-json/wp/v2/comments\n  status: 403\n  code: rest_comment_disabled\n  detail: Comments are disabled site-wide, so this collection is unreachable rather than credential-gated.\ncontext_escalation:\n  param: context\n  anonymous_values:\n  - view\n  - embed\n  gated_values:\n  - edit\n  detail: 'context=edit returns 401 rest_forbidden for an unauthenticated caller.'\ntransport:\n  https_only: true\n  tls_version: TLSv1.3\n  hsts: false\n  detail: >-\n    HTTPS is enforced at the edge (Cloudflare in front of WP Engine), but no Strict-Transport-Security\n    header is returned. See security/mbrace-therapeutics-domain-security.yml.\ncross_links:\n  conventions: conventions/mbrace-therapeutics-conventions.yml\n  errors: errors/mbrace-therapeutics-problem-types.yml\n  domain_security: security/mbrace-therapeutics-domain-security.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mbrace-therapeutics/refs/heads/main/authentication/mbrace-therapeutics-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Biotechnology
- Pharmaceuticals
- Oncology
- Antibody Drug Conjugates
- Drug Discovery
- Clinical Trials
- Life Sciences
- Precision Medicine
- content-api
---
