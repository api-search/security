---
api_key_in: []
api_specs:
- filename: cutiss-newsroom-api-openapi.yml
  format: yaml
  label: CUTISS Newsroom API
  slug: cutiss-newsroom-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cutiss/refs/heads/main/openapi/cutiss-newsroom-api-openapi.yml
- filename: cutiss-posts-api-openapi.yml
  format: yaml
  label: CUTISS Posts API
  slug: cutiss-posts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cutiss/refs/heads/main/openapi/cutiss-posts-api-openapi.yml
- filename: cutiss-pages-api-openapi.yml
  format: yaml
  label: CUTISS Pages API
  slug: cutiss-pages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cutiss/refs/heads/main/openapi/cutiss-pages-api-openapi.yml
- filename: cutiss-team-api-openapi.yml
  format: yaml
  label: CUTISS Team API
  slug: cutiss-team-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cutiss/refs/heads/main/openapi/cutiss-team-api-openapi.yml
- filename: cutiss-media-api-openapi.yml
  format: yaml
  label: CUTISS Media API
  slug: cutiss-media-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cutiss/refs/heads/main/openapi/cutiss-media-api-openapi.yml
- filename: cutiss-categories-api-openapi.yml
  format: yaml
  label: CUTISS Categories API
  slug: cutiss-categories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cutiss/refs/heads/main/openapi/cutiss-categories-api-openapi.yml
- filename: cutiss-search-api-openapi.yml
  format: yaml
  label: CUTISS Search API
  slug: cutiss-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cutiss/refs/heads/main/openapi/cutiss-search-api-openapi.yml
- filename: cutiss-teams-taxonomy-api-openapi.yml
  format: yaml
  label: CUTISS Teams Taxonomy API
  slug: cutiss-teams-taxonomy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cutiss/refs/heads/main/openapi/cutiss-teams-taxonomy-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
method: probed
name: Cutiss Authentication
name_suffix: Authentication
oauth_flows: []
overview: CUTISS declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: CUTISS
provider_slug: cutiss
scheme_count: 2
schemes:
- applies_to:
  - listPosts
  - listPages
  - listMedia
  - listCategories
  - listNewsroom
  - listTeam
  - listTeams
  - listSearch
  description: Anonymous GET on posts, pages, media, categories, newsroom2021, team_member, cutiss-teams, search, types, taxonomies and statuses. Verified 200 without credentials.
  name: none
  scope: public read
  type: none
- advertised: true
  description: 'WordPress core''s first-party authentication: a logged-in session cookie plus an X-WP-Nonce header. The header is advertised in Access-Control-Allow-Headers on every response. Only issued to authenticated CUTISS staff in wp-admin; there is no public registration, so this is not a usable scheme for a third-party integrator.'
  header: X-WP-Nonce
  in: header
  name: wordpress-cookie-nonce
  obtainable_by_public: false
  scope: write / privileged read
  type: apiKey
slug: cutiss-authentication
source_filename: cutiss-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-11'\nmethod: probed\nsource: https://cutiss.swiss/wp-json/ route index + live anonymous and unauthenticated probes\nsummary: 'The CUTISS content API is anonymous-read. No credential is required or accepted for the public\n  collections; every write method and every administrative collection is refused with HTTP 401 rest_forbidden.\n  The route index advertises no authentication method (\"authentication\": []), meaning no application-password\n  or OAuth provider is registered.'\nschemes:\n- name: none\n  type: none\n  scope: public read\n  description: Anonymous GET on posts, pages, media, categories, newsroom2021, team_member, cutiss-teams,\n    search, types, taxonomies and statuses. Verified 200 without credentials.\n  applies_to:\n  - listPosts\n  - listPages\n  - listMedia\n  - listCategories\n  - listNewsroom\n  - listTeam\n  - listTeams\n  - listSearch\n- name: wordpress-cookie-nonce\n  type: apiKey\n  in: header\n  header: X-WP-Nonce\n  scope: write\
  \ / privileged read\n  advertised: true\n  obtainable_by_public: false\n  description: 'WordPress core''s first-party authentication: a logged-in session cookie plus an X-WP-Nonce\n    header. The header is advertised in Access-Control-Allow-Headers on every response. Only issued to\n    authenticated CUTISS staff in wp-admin; there is no public registration, so this is not a usable scheme\n    for a third-party integrator.'\ngated_surfaces:\n- path: /wp/v2/users\n  status: 401\n  code: rest_forbidden\n- path: /wp/v2/settings\n  status: 401\n  code: rest_forbidden\n- path: /wp/v2/plugins\n  status: 401\n  code: rest_forbidden\n- path: /wp/v2/menus\n  status: 401\n  code: rest_forbidden\n- path: /wp/v2/block-types\n  status: 401\n  code: rest_forbidden\n- path: /wp-abilities/v1/abilities\n  status: 401\n  code: rest_forbidden\n- path: /wp-abilities/v1/categories\n  status: 401\n  code: rest_forbidden\noauth:\n  supported: false\n  note: No /.well-known/oauth-authorization-server and no\
  \ /.well-known/openid-configuration (both 404).\n    No OAuth scope surface exists, so no scopes/ artifact is written.\nregistration:\n  public_signup: false\n  note: CUTISS offers no developer account, API key issuance or sign-up flow of any kind.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cutiss/refs/heads/main/authentication/cutiss-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Biotechnology
- Regenerative Medicine
- Tissue Engineering
- Life Sciences
- Medical Devices
- Clinical Trials
- Dermatology
- Healthcare
- Switzerland
- Research
- Content
---
