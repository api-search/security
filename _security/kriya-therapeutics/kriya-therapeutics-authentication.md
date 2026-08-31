---
api_key_in:
- header
api_specs:
- filename: kriya-therapeutics-discovery-api-openapi.yml
  format: yaml
  label: Kriya Therapeutics Discovery API
  slug: kriya-therapeutics-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kriya-therapeutics/refs/heads/main/openapi/kriya-therapeutics-discovery-api-openapi.yml
- filename: kriya-therapeutics-forms-api-openapi.yml
  format: yaml
  label: Kriya Therapeutics Forms API
  slug: kriya-therapeutics-forms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kriya-therapeutics/refs/heads/main/openapi/kriya-therapeutics-forms-api-openapi.yml
- filename: kriya-therapeutics-media-api-openapi.yml
  format: yaml
  label: Kriya Therapeutics Media API
  slug: kriya-therapeutics-media-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kriya-therapeutics/refs/heads/main/openapi/kriya-therapeutics-media-api-openapi.yml
- filename: kriya-therapeutics-news-api-openapi.yml
  format: yaml
  label: Kriya Therapeutics News API
  slug: kriya-therapeutics-news-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kriya-therapeutics/refs/heads/main/openapi/kriya-therapeutics-news-api-openapi.yml
- filename: kriya-therapeutics-oembed-api-openapi.yml
  format: yaml
  label: Kriya Therapeutics Oembed API
  slug: kriya-therapeutics-oembed-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kriya-therapeutics/refs/heads/main/openapi/kriya-therapeutics-oembed-api-openapi.yml
- filename: kriya-therapeutics-pages-api-openapi.yml
  format: yaml
  label: Kriya Therapeutics Pages API
  slug: kriya-therapeutics-pages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kriya-therapeutics/refs/heads/main/openapi/kriya-therapeutics-pages-api-openapi.yml
- filename: kriya-therapeutics-posts-api-openapi.yml
  format: yaml
  label: Kriya Therapeutics Posts API
  slug: kriya-therapeutics-posts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kriya-therapeutics/refs/heads/main/openapi/kriya-therapeutics-posts-api-openapi.yml
- filename: kriya-therapeutics-search-api-openapi.yml
  format: yaml
  label: Kriya Therapeutics Search API
  slug: kriya-therapeutics-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kriya-therapeutics/refs/heads/main/openapi/kriya-therapeutics-search-api-openapi.yml
- filename: kriya-therapeutics-taxonomy-api-openapi.yml
  format: yaml
  label: Kriya Therapeutics Taxonomy API
  slug: kriya-therapeutics-taxonomy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kriya-therapeutics/refs/heads/main/openapi/kriya-therapeutics-taxonomy-api-openapi.yml
- filename: kriya-therapeutics-team-api-openapi.yml
  format: yaml
  label: Kriya Therapeutics Team API
  slug: kriya-therapeutics-team-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kriya-therapeutics/refs/heads/main/openapi/kriya-therapeutics-team-api-openapi.yml
auth_types:
- none
- apiKey
- http
description: ''
kind: authentication
layout: security
method: probed
name: Kriya Therapeutics Authentication
name_suffix: Authentication
oauth_flows: []
overview: Kriya Therapeutics secures its APIs with none, apiKey, and http across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Kriya Therapeutics
provider_slug: kriya-therapeutics
scheme_count: 3
schemes:
- applies_to:
  - getApiIndex
  - listNews
  - getNewsItem
  - listPosts
  - getPost
  - listPages
  - getPage
  - listTeam
  - listMedia
  - getMediaItem
  - listCategories
  - getCategory
  - listTags
  - listNewsCategories
  - listTeamKeywords
  - getTeamKeyword
  - listComments
  - listForms
  - searchContent
  - listTypes
  - getType
  - listTaxonomies
  - getTaxonomy
  - listStatuses
  - getOembed
  description: Every operation modelled in openapi/kriya-therapeutics-content-openapi.yml was verified to return data with no Authorization header, no cookie and no nonce. Read access is unrestricted and unmetered as observed.
  name: anonymous
  sources:
  - openapi/kriya-therapeutics-content-openapi.yml
  type: none
- description: WordPress core's first-party session scheme for same-origin browser requests. Inferred from the Access-Control-Allow-Headers response header observed on the collection endpoints, which lists 'Authorization, X-WP-Nonce, Content-Disposition, Content-MD5, Content-Type'. Not usable by a third-party integrator.
  in: header
  name: cookie-plus-nonce
  parameter_name: X-WP-Nonce
  sources:
  - https://kriyatherapeutics.com/wp-json/wp/v2/posts
  type: apiKey
- description: 'The CORS preflight allowlist includes `Authorization`, and the Wordfence namespace rejects anonymous calls with `rest_forbidden_context: Authorization header format is invalid.` — so an Authorization header is accepted and parsed by the deployment. Kriya Therapeutics advertises no method for obtaining such a credential (the REST index `authentication` array is empty), so this is an internal editorial credential, not a developer credential.'
  name: authorization-header
  scheme: unspecified
  sources:
  - https://kriyatherapeutics.com/wp-json/wordfence/v1/scan/issues
  - https://kriyatherapeutics.com/wp-json/wp/v2/posts
  type: http
slug: kriya-therapeutics-authentication
source_filename: kriya-therapeutics-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-04'\nmethod: probed\nsource: https://kriyatherapeutics.com/wp-json/ (REST API index) plus live anonymous requests on 2026-08-04\nnote: >-\n  The OpenAPI in this repo declares no securitySchemes because the operations it models are the ones\n  that genuinely return data with no credentials — the read side of the WordPress REST content API is\n  fully anonymous. This profile records that anonymous-read model and the authenticated surface that\n  sits behind it. Note that unlike most WordPress deployments, the `authentication` block in this\n  site's own REST index is an EMPTY array: Kriya Therapeutics advertises no authentication method at\n  all, so the gated routes below return 401 with no advertised way for a third party to authenticate.\n  Kriya Therapeutics publishes no developer authentication documentation of its own; the schemes\n  below are WordPress core behaviour observed on the wire.\nsummary:\n  types: [none, apiKey, http]\n  anonymous_read: true\n\
  \  api_key_in: [header]\n  oauth2_flows: []\n  oauth2: false\n  openid_connect: false\n  advertised_by_provider: false\nschemes:\n- name: anonymous\n  type: none\n  description: >-\n    Every operation modelled in openapi/kriya-therapeutics-content-openapi.yml was verified to return\n    data with no Authorization header, no cookie and no nonce. Read access is unrestricted and\n    unmetered as observed.\n  applies_to:\n  - getApiIndex\n  - listNews\n  - getNewsItem\n  - listPosts\n  - getPost\n  - listPages\n  - getPage\n  - listTeam\n  - listMedia\n  - getMediaItem\n  - listCategories\n  - getCategory\n  - listTags\n  - listNewsCategories\n  - listTeamKeywords\n  - getTeamKeyword\n  - listComments\n  - listForms\n  - searchContent\n  - listTypes\n  - getType\n  - listTaxonomies\n  - getTaxonomy\n  - listStatuses\n  - getOembed\n  sources: [openapi/kriya-therapeutics-content-openapi.yml]\n- name: cookie-plus-nonce\n  type: apiKey\n  in: header\n  parameter_name: X-WP-Nonce\n  description:\
  \ >-\n    WordPress core's first-party session scheme for same-origin browser requests. Inferred from the\n    Access-Control-Allow-Headers response header observed on the collection endpoints, which lists\n    'Authorization, X-WP-Nonce, Content-Disposition, Content-MD5, Content-Type'. Not usable by a\n    third-party integrator.\n  sources: [https://kriyatherapeutics.com/wp-json/wp/v2/posts]\n- name: authorization-header\n  type: http\n  scheme: unspecified\n  description: >-\n    The CORS preflight allowlist includes `Authorization`, and the Wordfence namespace rejects\n    anonymous calls with `rest_forbidden_context: Authorization header format is invalid.` — so an\n    Authorization header is accepted and parsed by the deployment. Kriya Therapeutics advertises no\n    method for obtaining such a credential (the REST index `authentication` array is empty), so this\n    is an internal editorial credential, not a developer credential.\n  sources:\n  - https://kriyatherapeutics.com/wp-json/wordfence/v1/scan/issues\n\
  \  - https://kriyatherapeutics.com/wp-json/wp/v2/posts\ngated_surfaces:\n- path: /wp/v2/settings\n  status: 401\n  code: rest_forbidden\n- path: /wp/v2/users\n  status: 401\n  code: rest_user_cannot_view\n  note: Author records are not readable anonymously on this deployment, unlike WordPress default.\n- path: /wp/v2/themes\n  status: 401\n  code: rest_cannot_view_themes\n- path: /wp/v2/plugins\n  status: 401\n  code: rest_cannot_view_plugins\n- path: /wp/v2/menus\n  status: 401\n  code: rest_cannot_view\n- path: /wp/v2/block-types\n  status: 401\n  code: rest_block_type_cannot_view\n- path: /wp-abilities/v1/abilities\n  status: 401\n  code: rest_forbidden\n  note: >-\n    The WordPress Abilities API — an agent-facing capability registry with a /run execution\n    endpoint — is registered on this site but is entirely credential-gated. No agent capability is\n    exposed to anonymous callers, so no MCP or agent-surface claim is made for this provider.\n- path: /wp-abilities/v1/categories\n\
  \  status: 401\n  code: rest_forbidden\n- path: /gutena-forms/v1/forms/get-all\n  status: 401\n  code: rest_forbidden\n  note: Form definitions are readable via /wp/v2/gutena_forms, but the plugin's own form and ENTRY endpoints are gated — submitted form entries are not exposed anonymously.\n- path: /gutena-forms/v1/settings\n  status: 401\n  code: rest_forbidden\n- path: /yoast/v1/statistics\n  status: 401\n  code: rest_forbidden\n- path: /wordfence/v1/scan/issues\n  status: 401\n  code: rest_forbidden_context\n  note: 'Message reads \"Authorization header format is invalid.\" — the Wordfence security plugin namespace is registered and credential-gated.'\n- path: /wp-site-health/v1/tests/https-status\n  status: 401\n  code: rest_forbidden\n- path: /wpe_sign_on_plugin/v1/is_user_logged_in\n  status: 307\n  note: WP Engine single-sign-on plugin route; redirects rather than answering anonymously.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kriya-therapeutics/refs/heads/main/authentication/kriya-therapeutics-authentication.yml
summary_line: none/apiKey/http · 3 schemes
tags:
- Company
- biotechnology
- pharmaceuticals
- gene-therapy
- aav
- ophthalmology
- metabolic-disease
- neurology
- life-sciences
- clinical-trials
- biomanufacturing
- content-api
---
