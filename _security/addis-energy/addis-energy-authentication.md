---
anonymous_access: true
api_key_in: []
api_specs:
- filename: addis-energy-posts-api-openapi.yml
  format: yaml
  label: Addis Energy Posts API
  slug: addis-energy-posts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/addis-energy/refs/heads/main/openapi/addis-energy-posts-api-openapi.yml
- filename: addis-energy-pages-api-openapi.yml
  format: yaml
  label: Addis Energy Pages API
  slug: addis-energy-pages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/addis-energy/refs/heads/main/openapi/addis-energy-pages-api-openapi.yml
- filename: addis-energy-media-api-openapi.yml
  format: yaml
  label: Addis Energy Media API
  slug: addis-energy-media-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/addis-energy/refs/heads/main/openapi/addis-energy-media-api-openapi.yml
- filename: addis-energy-taxonomy-api-openapi.yml
  format: yaml
  label: Addis Energy Taxonomy API
  slug: addis-energy-taxonomy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/addis-energy/refs/heads/main/openapi/addis-energy-taxonomy-api-openapi.yml
- filename: addis-energy-users-api-openapi.yml
  format: yaml
  label: Addis Energy Users API
  slug: addis-energy-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/addis-energy/refs/heads/main/openapi/addis-energy-users-api-openapi.yml
- filename: addis-energy-search-api-openapi.yml
  format: yaml
  label: Addis Energy Search API
  slug: addis-energy-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/addis-energy/refs/heads/main/openapi/addis-energy-search-api-openapi.yml
- filename: addis-energy-discovery-api-openapi.yml
  format: yaml
  label: Addis Energy Discovery API
  slug: addis-energy-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/addis-energy/refs/heads/main/openapi/addis-energy-discovery-api-openapi.yml
- filename: addis-energy-oembed-api-openapi.yml
  format: yaml
  label: Addis Energy oEmbed API
  slug: addis-energy-oembed-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/addis-energy/refs/heads/main/openapi/addis-energy-oembed-api-openapi.yml
auth_types: []
description: Authentication profile for the WordPress core REST API behind addisenergy.com. There is no developer program, no signup, no API key issuance and no OAuth server. The public surface is anonymous and read-only; the write half of the same routes is gated by WordPress application passwords, which only an existing site administrator can mint from wp-admin.
kind: authentication
layout: security
mechanism_count: 1
method: probed
name: Addis Energy Authentication
name_suffix: Authentication
oauth_flows: []
overview: Addis Energy declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Addis Energy
provider_slug: addis-energy
scheme_count: 2
schemes:
- applies_to: every GET operation in openapi/
  description: All eight APIs profiled here are readable with no credential. This is the entire public surface.
  id: none
  name: Anonymous
  type: none
  verified: 2026-09-07
- applies_to: The POST/PUT/PATCH/DELETE half of the wp/v2 routes, plus the entirety of the contact-form-7/v1, code-snippets/v1, siteground-optimizer/v1, duplicator/v1 and wp-abilities/v1 namespaces.
  authorization_endpoint: https://addisenergy.com/wp-admin/authorize-application.php
  description: 'HTTP Basic with a WordPress username and an application password, declared by the server''s own discovery document at https://addisenergy.com/wp-json/ under `authentication`. This is the only authentication method the site advertises. It is NOT a developer credential: application passwords are minted per-user from wp-admin by a signed-in site administrator, so there is no path for a third party to obtain one.'
  id: application-passwords
  name: WordPress application passwords
  public_issuance: false
  scheme: basic
  type: http
  verified: 2026-09-07
slug: addis-energy-authentication
source_filename: addis-energy-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-07'\nmethod: probed\nsource: https://addisenergy.com/wp-json/ (authentication block of the live route index) plus live anonymous requests to every route in openapi/\ndescription: >-\n  Authentication profile for the WordPress core REST API behind addisenergy.com. There is no\n  developer program, no signup, no API key issuance and no OAuth server. The public surface is\n  anonymous and read-only; the write half of the same routes is gated by WordPress application\n  passwords, which only an existing site administrator can mint from wp-admin.\napis:\n- addis-energy:addis-energy-posts-api\n- addis-energy:addis-energy-pages-api\n- addis-energy:addis-energy-media-api\n- addis-energy:addis-energy-taxonomy-api\n- addis-energy:addis-energy-users-api\n- addis-energy:addis-energy-search-api\n- addis-energy:addis-energy-discovery-api\n- addis-energy:addis-energy-oembed-api\nanonymous_access:\n  supported: true\n  scope: read-only\n  evidence: >-\n    GET https://addisenergy.com/wp-json/wp/v2/posts?per_page=1\
  \ returned HTTP 200 with\n    `Allow: GET` and `X-WP-Total: 13` on 2026-09-07 with no credentials of any kind.\n  note: >-\n    The public projection is limited to the WordPress `view` context. Anonymous callers see\n    published objects only; no draft, private or edit-context field is returned.\nschemes:\n- id: none\n  type: none\n  name: Anonymous\n  description: >-\n    All eight APIs profiled here are readable with no credential. This is the entire public\n    surface.\n  applies_to: every GET operation in openapi/\n  verified: 2026-09-07\n- id: application-passwords\n  type: http\n  scheme: basic\n  name: WordPress application passwords\n  description: >-\n    HTTP Basic with a WordPress username and an application password, declared by the server's own\n    discovery document at https://addisenergy.com/wp-json/ under `authentication`. This is the only\n    authentication method the site advertises. It is NOT a developer credential: application\n    passwords are minted per-user\
  \ from wp-admin by a signed-in site administrator, so there is no\n    path for a third party to obtain one.\n  authorization_endpoint: https://addisenergy.com/wp-admin/authorize-application.php\n  applies_to: >-\n    The POST/PUT/PATCH/DELETE half of the wp/v2 routes, plus the entirety of the\n    contact-form-7/v1, code-snippets/v1, siteground-optimizer/v1, duplicator/v1 and\n    wp-abilities/v1 namespaces.\n  public_issuance: false\n  verified: 2026-09-07\ngated_surfaces:\n- route: /wp/v2/settings\n  status: 401\n  code: rest_forbidden\n  note: Site settings require an authenticated administrator.\n- route: /wp-abilities/v1/abilities\n  status: 401\n  code: rest_forbidden\n  note: The WordPress Abilities API is registered but administrator-only; no ability is anonymously enumerable.\n- route: /contact-form-7/v1/contact-forms\n  status: 403\n  code: wpcf7_forbidden\n  note: Contact Form 7 form definitions are not public. The public contact form posts to /feedback, which is not a documented\
  \ integration surface.\n- route: /wp/v2/comments\n  status: 403\n  code: rest_comment_disabled\n  note: Comments are disabled site-wide, so the comments collection is unavailable even anonymously.\nnot_present:\n  oauth2: false\n  openid_connect: false\n  mutual_tls: false\n  api_keys: false\n  jwt: false\n  note: >-\n    No OAuth authorization server, no OpenID Connect discovery document and no API-key programme\n    exist. /.well-known/openid-configuration and /.well-known/oauth-authorization-server both\n    returned 404 on 2026-09-07. scopes/ is therefore not applicable and is deliberately not emitted.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/addis-energy/refs/heads/main/authentication/addis-energy-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Energy
- Clean Energy
- Ammonia
- Climate Tech
- Deep Tech
- Geoscience
- Subsurface
- Materials Science
- Hydrogen
- Fertilizer
- Content
---
