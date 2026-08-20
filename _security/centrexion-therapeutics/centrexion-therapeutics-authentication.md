---
api_key_in: []
api_specs:
- filename: centrexion-therapeutics-comments-api-openapi.yml
  format: yaml
  label: Centrexion Therapeutics Comments API
  slug: centrexion-therapeutics-comments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/centrexion-therapeutics/refs/heads/main/openapi/centrexion-therapeutics-comments-api-openapi.yml
- filename: centrexion-therapeutics-custom-types-api-openapi.yml
  format: yaml
  label: Centrexion Therapeutics Custom Types API
  slug: centrexion-therapeutics-custom-types-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/centrexion-therapeutics/refs/heads/main/openapi/centrexion-therapeutics-custom-types-api-openapi.yml
- filename: centrexion-therapeutics-discovery-api-openapi.yml
  format: yaml
  label: Centrexion Therapeutics Discovery API
  slug: centrexion-therapeutics-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/centrexion-therapeutics/refs/heads/main/openapi/centrexion-therapeutics-discovery-api-openapi.yml
- filename: centrexion-therapeutics-media-api-openapi.yml
  format: yaml
  label: Centrexion Therapeutics Media API
  slug: centrexion-therapeutics-media-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/centrexion-therapeutics/refs/heads/main/openapi/centrexion-therapeutics-media-api-openapi.yml
- filename: centrexion-therapeutics-oembed-api-openapi.yml
  format: yaml
  label: Centrexion Therapeutics Oembed API
  slug: centrexion-therapeutics-oembed-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/centrexion-therapeutics/refs/heads/main/openapi/centrexion-therapeutics-oembed-api-openapi.yml
- filename: centrexion-therapeutics-pages-api-openapi.yml
  format: yaml
  label: Centrexion Therapeutics Pages API
  slug: centrexion-therapeutics-pages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/centrexion-therapeutics/refs/heads/main/openapi/centrexion-therapeutics-pages-api-openapi.yml
- filename: centrexion-therapeutics-people-api-openapi.yml
  format: yaml
  label: Centrexion Therapeutics People API
  slug: centrexion-therapeutics-people-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/centrexion-therapeutics/refs/heads/main/openapi/centrexion-therapeutics-people-api-openapi.yml
- filename: centrexion-therapeutics-posts-api-openapi.yml
  format: yaml
  label: Centrexion Therapeutics Posts API
  slug: centrexion-therapeutics-posts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/centrexion-therapeutics/refs/heads/main/openapi/centrexion-therapeutics-posts-api-openapi.yml
- filename: centrexion-therapeutics-search-api-openapi.yml
  format: yaml
  label: Centrexion Therapeutics Search API
  slug: centrexion-therapeutics-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/centrexion-therapeutics/refs/heads/main/openapi/centrexion-therapeutics-search-api-openapi.yml
- filename: centrexion-therapeutics-taxonomy-api-openapi.yml
  format: yaml
  label: Centrexion Therapeutics Taxonomy API
  slug: centrexion-therapeutics-taxonomy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/centrexion-therapeutics/refs/heads/main/openapi/centrexion-therapeutics-taxonomy-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
method: derived
name: Centrexion Therapeutics Authentication
name_suffix: Authentication
oauth_flows: []
overview: Centrexion Therapeutics declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Centrexion Therapeutics
provider_slug: centrexion-therapeutics
scheme_count: 1
schemes:
- applies_to: write and administrative routes (not modelled)
  authorization_endpoint: https://centrexion.com/wp-admin/authorize-application.php
  description: WordPress application passwords, sent as HTTP Basic credentials. Advertised in the REST index `authentication` object. Governs write and administrative routes only; not required by, and not applicable to, any operation modelled in this repo.
  name: applicationPassword
  scheme: basic
  sources:
  - https://centrexion.com/wp-json/
  type: http
slug: centrexion-therapeutics-authentication
source_filename: centrexion-therapeutics-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-09'\nmethod: derived\nsource: openapi/centrexion-therapeutics-content-openapi.yml + live probes of https://centrexion.com/wp-json/\nsummary:\n  types: []\n  api_key_in: []\n  oauth2_flows: []\n  anonymous_read: true\nnote: >-\n  The Centrexion Therapeutics content API declares NO security schemes for the operations catalogued\n  in this repo, because every catalogued operation is anonymously readable. This is not an omission\n  in the derivation — it is the actual posture of the surface. The site index at\n  https://centrexion.com/wp-json/ advertises exactly one registered authentication method,\n  WordPress application passwords, whose authorization endpoint is\n  https://centrexion.com/wp-admin/authorize-application.php. That mechanism gates the write and\n  administrative surface, which this repo deliberately does not model. There is no OAuth 2.0\n  authorization server, no OpenID Connect discovery document, no API-key programme, no developer\n  key issuance,\
  \ and no scope model — /.well-known/oauth-authorization-server and\n  /.well-known/openid-configuration both return 404 (see\n  well-known/centrexion-therapeutics-well-known.yml). Consequently there is no scopes/ artifact for\n  this provider: OAuth scopes require an OAuth surface, and none exists.\nschemes:\n- name: applicationPassword\n  type: http\n  scheme: basic\n  description: >-\n    WordPress application passwords, sent as HTTP Basic credentials. Advertised in the REST index\n    `authentication` object. Governs write and administrative routes only; not required by, and not\n    applicable to, any operation modelled in this repo.\n  authorization_endpoint: https://centrexion.com/wp-admin/authorize-application.php\n  applies_to: write and administrative routes (not modelled)\n  sources: [https://centrexion.com/wp-json/]\nanonymous_surface:\n  description: >-\n    Operations verified to return data with no credentials on 2026-08-09. These are the operations\n    modelled in openapi/centrexion-therapeutics-content-openapi.yml.\n\
  \  operations:\n  - getApiIndex\n  - listPosts\n  - getPost\n  - listPages\n  - getPage\n  - listMedia\n  - getMediaItem\n  - listCategories\n  - getCategory\n  - listTags\n  - listPostSeries\n  - listComments\n  - getComment\n  - search\n  - listUsers\n  - listNavigation\n  - getNavigation\n  - listReusableBlocks\n  - listDynamicTemplates\n  - listCustomCards\n  - listPostTypes\n  - getPostType\n  - listTaxonomies\n  - getTaxonomy\n  - listStatuses\n  - getStatus\n  - getOembed\ngated_surface:\n  description: >-\n    Routes that exist in the published route index but returned 401 to an anonymous caller on\n    2026-08-09, with the WordPress error code each returned. Recorded so the boundary between the\n    public and credentialed surface is explicit; none of these are modelled in the OpenAPI.\n  routes:\n  - {path: /wp/v2/settings, status: 401, code: rest_forbidden}\n  - {path: /wp/v2/menus, status: 401, code: rest_cannot_view}\n  - {path: /wp/v2/menu-locations, status: 401, code: rest_cannot_view}\n\
  \  - {path: /wp/v2/icons, status: 401, code: rest_cannot_view}\n  - {path: /wp/v2/block-patterns/categories, status: 401, code: rest_cannot_view}\n  - {path: /wp/v2/themes, status: 401, code: rest_cannot_view_themes}\n  - {path: /wp/v2/plugins, status: 401, code: rest_cannot_view_plugins}\n  - {path: /wp/v2/block-types, status: 401, code: rest_block_type_cannot_view}\n  - {path: /wp/v2/font-collections, status: 401, code: rest_cannot_read}\n  - {path: /wp/v2/sidebars, status: 401, code: rest_cannot_manage_widgets}\n  - {path: /wp/v2/widget-types, status: 401, code: rest_cannot_manage_widgets}\n  - {path: /wp/v2/pattern-directory/patterns, status: 401, code: rest_pattern_directory_cannot_view}\n  - {path: /wp-abilities/v1/abilities, status: 401, code: rest_forbidden}\n  - {path: /wp-abilities/v1/categories, status: 401, code: rest_forbidden}\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/centrexion-therapeutics/refs/heads/main/authentication/centrexion-therapeutics-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Biopharmaceutical
- Pharmaceuticals
- Chronic Pain
- non-opioid-analgesics
- Immunology
- inflammation
- Clinical Trials
- Life Sciences
- content-api
---
