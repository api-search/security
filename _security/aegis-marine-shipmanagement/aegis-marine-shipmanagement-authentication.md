---
anonymous_access: false
api_key_in: []
api_specs:
- filename: aegis-marine-shipmanagement-pages-api-openapi.yml
  format: yaml
  label: Aegis Marine Shipmanagement Pages API
  slug: aegis-marine-shipmanagement-pages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aegis-marine-shipmanagement/refs/heads/main/openapi/aegis-marine-shipmanagement-pages-api-openapi.yml
- filename: aegis-marine-shipmanagement-media-api-openapi.yml
  format: yaml
  label: Aegis Marine Shipmanagement Media API
  slug: aegis-marine-shipmanagement-media-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aegis-marine-shipmanagement/refs/heads/main/openapi/aegis-marine-shipmanagement-media-api-openapi.yml
- filename: aegis-marine-shipmanagement-taxonomy-api-openapi.yml
  format: yaml
  label: Aegis Marine Shipmanagement Taxonomy API
  slug: aegis-marine-shipmanagement-taxonomy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aegis-marine-shipmanagement/refs/heads/main/openapi/aegis-marine-shipmanagement-taxonomy-api-openapi.yml
- filename: aegis-marine-shipmanagement-search-api-openapi.yml
  format: yaml
  label: Aegis Marine Shipmanagement Search API
  slug: aegis-marine-shipmanagement-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aegis-marine-shipmanagement/refs/heads/main/openapi/aegis-marine-shipmanagement-search-api-openapi.yml
- filename: aegis-marine-shipmanagement-discovery-api-openapi.yml
  format: yaml
  label: Aegis Marine Shipmanagement Discovery API
  slug: aegis-marine-shipmanagement-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aegis-marine-shipmanagement/refs/heads/main/openapi/aegis-marine-shipmanagement-discovery-api-openapi.yml
- filename: aegis-marine-shipmanagement-oembed-api-openapi.yml
  format: yaml
  label: Aegis Marine Shipmanagement oEmbed API
  slug: aegis-marine-shipmanagement-oembed-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aegis-marine-shipmanagement/refs/heads/main/openapi/aegis-marine-shipmanagement-oembed-api-openapi.yml
- filename: aegis-marine-shipmanagement-seo-api-openapi.yml
  format: yaml
  label: Aegis Marine Shipmanagement SEO Metadata API
  slug: aegis-marine-shipmanagement-seo-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aegis-marine-shipmanagement/refs/heads/main/openapi/aegis-marine-shipmanagement-seo-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 0
method: probed
name: Aegis Marine Shipmanagement Authentication
name_suffix: Authentication
oauth_flows: []
overview: Aegis Marine Shipmanagement declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: Aegis Marine Shipmanagement
provider_slug: aegis-marine-shipmanagement
scheme_count: 0
schemes: []
slug: aegis-marine-shipmanagement-authentication
source_filename: aegis-marine-shipmanagement-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-09'\nmethod: probed\nsource: >-\n  Live anonymous probes of https://aegisships.com/wp-json/ and its collections, 2026-09-09. The\n  root index advertises an empty `authentication` array; no developer documentation, signup, key\n  issuance or OAuth surface exists on aegisships.com.\nprovider: Aegis Marine Shipmanagement\nsummary: >-\n  The entire publicly reachable surface is anonymous and unauthenticated. Aegis Marine\n  Shipmanagement operates no developer program: there is no signup, no API key issuance, no OAuth\n  client registration and no documented credential of any kind. Reads against published content\n  succeed with no credentials; the routes that would require a credential are simply closed to the\n  public, returning HTTP 401 rather than offering a way to authenticate.\nschemes: []\nschemes_note: >-\n  No securityScheme is declared, because none is served. The derived OpenAPI documents in openapi/\n  intentionally carry no `securitySchemes` block\
  \ — inventing one would assert an authentication\n  model this provider does not publish.\nanonymous_access:\n  supported: true\n  scope: read-only\n  credential_required: false\n  verified: '2026-09-09'\n  evidence:\n  - url: https://aegisships.com/wp-json/\n    status: 200\n    note: Root index returns `\"authentication\":[]` — no scheme advertised.\n  - url: https://aegisships.com/wp-json/wp/v2/pages?per_page=1\n    status: 200\n    note: 15 pages readable with no credential (X-WP-Total 15).\n  - url: https://aegisships.com/wp-json/wp/v2/media?per_page=1\n    status: 200\n    note: 121 attachments readable with no credential.\ngated_surfaces:\n- path: /wp/v2/users\n  status: 401\n  code: rest_user_cannot_view\n  note: >-\n    User enumeration is denied. Page and media records carry an `author` integer that therefore\n    cannot be resolved anonymously.\n- path: /wp/v2/settings\n  status: 401\n  code: rest_forbidden\n  note: Site settings require an authenticated administrator.\n- path:\
  \ /contact-form-7/v1/contact-forms\n  status: 403\n  code: wpcf7_forbidden\n  note: Contact Form 7 form definitions are not publicly listable.\nwrite_surface:\n  publicly_available: false\n  note: >-\n    The route index registers POST/PUT/PATCH/DELETE methods on core WordPress collections, and\n    admin namespaces (wordfence/v1, yoast/v1 indexing, wp-site-health/v1) are present. None is\n    usable by the public: WordPress applies the same capability checks that return 401 on\n    /wp/v2/settings, and no credential can be obtained because no signup exists. The derived\n    OpenAPI documents scope to the anonymously reachable GET surface for this reason.\n  supported_credentials_upstream:\n  - Application Passwords (/wp/v2/users/{id}/application-passwords) — registered by WordPress core\n    but requires an existing authenticated account; no account provisioning is offered publicly.\nrecommendations:\n- Aegis Marine Shipmanagement publishes no authentication documentation because it offers\
  \ no\n  developer program; nothing here should be read as a gap in a product they sell.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aegis-marine-shipmanagement/refs/heads/main/authentication/aegis-marine-shipmanagement-authentication.yml
summary_line: 0 schemes
tags:
- Company
- Shipping
- Ship Management
- Maritime
- Marine Transportation
- Oil and Gas
- Crude Oil Tankers
- LNG
- Offshore
- Chartering
- Crew Management
- Logistics
- Guyana
- Content
---
