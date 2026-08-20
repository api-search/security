---
api_key_in: []
api_specs:
- filename: recode-therapeutics-content-api-openapi.yml
  format: yaml
  label: ReCode Therapeutics Content API
  slug: recode-therapeutics-content-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/recode-therapeutics/refs/heads/main/openapi/recode-therapeutics-content-api-openapi.yml
- filename: recode-therapeutics-discovery-api-openapi.yml
  format: yaml
  label: ReCode Therapeutics Discovery API
  slug: recode-therapeutics-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/recode-therapeutics/refs/heads/main/openapi/recode-therapeutics-discovery-api-openapi.yml
- filename: recode-therapeutics-embed-api-openapi.yml
  format: yaml
  label: ReCode Therapeutics Embed API
  slug: recode-therapeutics-embed-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/recode-therapeutics/refs/heads/main/openapi/recode-therapeutics-embed-api-openapi.yml
- filename: recode-therapeutics-media-api-openapi.yml
  format: yaml
  label: ReCode Therapeutics Media API
  slug: recode-therapeutics-media-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/recode-therapeutics/refs/heads/main/openapi/recode-therapeutics-media-api-openapi.yml
- filename: recode-therapeutics-people-api-openapi.yml
  format: yaml
  label: ReCode Therapeutics People API
  slug: recode-therapeutics-people-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/recode-therapeutics/refs/heads/main/openapi/recode-therapeutics-people-api-openapi.yml
- filename: recode-therapeutics-search-api-openapi.yml
  format: yaml
  label: ReCode Therapeutics Search API
  slug: recode-therapeutics-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/recode-therapeutics/refs/heads/main/openapi/recode-therapeutics-search-api-openapi.yml
- filename: recode-therapeutics-taxonomy-api-openapi.yml
  format: yaml
  label: ReCode Therapeutics Taxonomy API
  slug: recode-therapeutics-taxonomy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/recode-therapeutics/refs/heads/main/openapi/recode-therapeutics-taxonomy-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
method: derived
name: Recode Therapeutics Authentication
name_suffix: Authentication
oauth_flows: []
overview: ReCode Therapeutics declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: ReCode Therapeutics
provider_slug: recode-therapeutics
scheme_count: 0
schemes: []
slug: recode-therapeutics-authentication
source_filename: recode-therapeutics-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-05'\nmethod: derived\nsource: openapi/recode-therapeutics-content-openapi.yml\nsummary: >-\n  The ReCode Therapeutics content API has NO consumer authentication. Every operation catalogued in\n  this repository was verified to return 200 anonymously with no header, no key, no token and no\n  cookie. There is no signup, no key issuance, no developer account and no rate-limit tier, because\n  ReCode Therapeutics does not run a developer program — this is the site's own WordPress REST\n  surface, left open by default.\nmodel: none\npublic_read: true\nschemes: []\ndeclared_but_unusable:\n  - scheme: application-passwords\n    advertised_at: https://recodetx.com/wp-json/\n    field: authentication[\"application-passwords\"].endpoints.authorization\n    authorization_endpoint: https://recodetx.com/wp-admin/authorize-application.php\n    usable_by_public: false\n    note: >-\n      The root index advertises WordPress Application Passwords. This is NOT a public\
  \ API credential\n      — it is an interactive flow that requires an existing wp-admin account on the site to\n      approve. No unauthenticated consumer can obtain one, so it confers no additional access and is\n      recorded here only because the install advertises it.\nauthorization_boundary:\n  description: >-\n    What the anonymous boundary actually gates, observed 2026-08-05. Read access to published\n    content is open; everything administrative is closed.\n  open_anonymously:\n    - /wp/v2/posts, /wp/v2/pages, /wp/v2/media\n    - /wp/v2/events, /wp/v2/values (site-specific custom post types)\n    - /wp/v2/categories, /wp/v2/tags, /wp/v2/types, /wp/v2/statuses, /wp/v2/taxonomies\n    - /wp/v2/search, /wp/v2/comments (empty)\n    - /wp/v2/users (5 records — see the personal-data note below)\n    - /oembed/1.0/embed\n  closed_401:\n    - path: /wp/v2/settings\n      code: rest_forbidden\n    - path: /wp/v2/menu-items\n      code: rest_cannot_view\n    - path: /wp/v2/themes\n  \
  \    code: rest_cannot_view_themes\n    - path: /wp/v2/plugins\n      code: rest_cannot_view_plugins\n    - path: /wp/v2/templates\n      code: rest_cannot_manage_templates\n    - path: /wp/v2/block-patterns/patterns\n      code: rest_cannot_view\n    - path: /wp/v2/font-families\n      code: rest_cannot_read\n    - path: /wp/v2/elementor_library\n      code: rest_forbidden\n    - path: /wp-json/aioseo/v1/*\n      code: rest_forbidden\n    - path: /wp-json/elementor/v1/*, /wp-json/elementor-pro/v1/*, /wp-json/elementor-ai/v1/*\n      code: rest_forbidden\n    - path: /wp-json/redirection/v1/*\n      code: rest_forbidden\n    - path: /wp-json/wp-site-health/v1/*\n      code: rest_forbidden\n    - path: /wp-json/wp-abilities/v1/abilities\n      code: rest_forbidden\n      note: >-\n        The install registers the WordPress Abilities API — an agent-facing capability registry —\n        but it is closed to anonymous callers, so no agent surface is claimed for this provider.\n  write_operations:\
  \ >-\n    All POST/PUT/PATCH/DELETE routes are registered by WordPress but require an authenticated,\n    capability-bearing user. None are reachable by a public consumer and none are modelled in the\n    OpenAPI.\npersonal_data_note: >-\n  /wp/v2/users returns 200 anonymously with 5 author records (display name, slug, description,\n  public profile link, Gravatar URLs). Email addresses and roles are not exposed. API Evangelist\n  documents the exposure but packages no agent skill or MCP tool against it and names no\n  individual. If author enumeration is unintended, ReCode Therapeutics can close the collection\n  with a rest_endpoints filter or the equivalent WP Engine / security-plugin setting.\ndocs: null\ndocs_note: >-\n  ReCode Therapeutics publishes no authentication documentation because it publishes no developer\n  documentation at all. The governing contract is the upstream WordPress REST Handbook:\n  https://developer.wordpress.org/rest-api/using-the-rest-api/authentication/\n\
  x-evidence:\n  verified: '2026-08-05'\n  method: anonymous HTTP GET against every route, recording the status and error code returned\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/recode-therapeutics/refs/heads/main/authentication/recode-therapeutics-authentication.yml
summary_line: 0 schemes
tags:
- Company
- Genetic Medicines
- Biotechnology
- biopharmaceuticals
- mRNA
- gene-correction
- Lipid Nanoparticles
- Drug Delivery
- Rare Disease
- cystic-fibrosis
- primary-ciliary-dyskinesia
- Clinical Trials
- Life Sciences
- content-api
---
