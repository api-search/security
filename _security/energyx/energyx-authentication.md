---
api_key_in: []
api_specs:
- filename: energyx-posts-api-openapi.yml
  format: yaml
  label: EnergyX Posts API
  slug: energyx-posts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/energyx/refs/heads/main/openapi/energyx-posts-api-openapi.yml
- filename: energyx-pages-api-openapi.yml
  format: yaml
  label: EnergyX Pages API
  slug: energyx-pages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/energyx/refs/heads/main/openapi/energyx-pages-api-openapi.yml
- filename: energyx-press-api-openapi.yml
  format: yaml
  label: EnergyX Press and News API
  slug: energyx-press-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/energyx/refs/heads/main/openapi/energyx-press-api-openapi.yml
- filename: energyx-leadership-api-openapi.yml
  format: yaml
  label: EnergyX Leadership API
  slug: energyx-leadership-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/energyx/refs/heads/main/openapi/energyx-leadership-api-openapi.yml
- filename: energyx-careers-api-openapi.yml
  format: yaml
  label: EnergyX Careers API
  slug: energyx-careers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/energyx/refs/heads/main/openapi/energyx-careers-api-openapi.yml
- filename: energyx-partners-api-openapi.yml
  format: yaml
  label: EnergyX Partners API
  slug: energyx-partners-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/energyx/refs/heads/main/openapi/energyx-partners-api-openapi.yml
- filename: energyx-videos-api-openapi.yml
  format: yaml
  label: EnergyX Videos API
  slug: energyx-videos-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/energyx/refs/heads/main/openapi/energyx-videos-api-openapi.yml
- filename: energyx-resource-guides-api-openapi.yml
  format: yaml
  label: EnergyX Resource Guides API
  slug: energyx-resource-guides-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/energyx/refs/heads/main/openapi/energyx-resource-guides-api-openapi.yml
- filename: energyx-media-api-openapi.yml
  format: yaml
  label: EnergyX Media API
  slug: energyx-media-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/energyx/refs/heads/main/openapi/energyx-media-api-openapi.yml
- filename: energyx-taxonomy-api-openapi.yml
  format: yaml
  label: EnergyX Taxonomy API
  slug: energyx-taxonomy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/energyx/refs/heads/main/openapi/energyx-taxonomy-api-openapi.yml
- filename: energyx-search-api-openapi.yml
  format: yaml
  label: EnergyX Search API
  slug: energyx-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/energyx/refs/heads/main/openapi/energyx-search-api-openapi.yml
- filename: energyx-discovery-api-openapi.yml
  format: yaml
  label: EnergyX Discovery API
  slug: energyx-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/energyx/refs/heads/main/openapi/energyx-discovery-api-openapi.yml
- filename: energyx-store-api-openapi.yml
  format: yaml
  label: EnergyX Store API
  slug: energyx-store-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/energyx/refs/heads/main/openapi/energyx-store-api-openapi.yml
- filename: energyx-oembed-api-openapi.yml
  format: yaml
  label: EnergyX oEmbed API
  slug: energyx-oembed-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/energyx/refs/heads/main/openapi/energyx-oembed-api-openapi.yml
- filename: energyx-seo-api-openapi.yml
  format: yaml
  label: EnergyX SEO Metadata API
  slug: energyx-seo-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/energyx/refs/heads/main/openapi/energyx-seo-api-openapi.yml
auth_types: []
description: EnergyX publishes no developer program and issues no API credentials. The WordPress REST content API behind energyx.com is anonymously readable — no key, token, signature or account is required to read posts, pages, press releases, in-the-news coverage, leadership, job positions, partners, videos, resource guides, media, taxonomies, search, the storefront catalog or the discovery metadata. The server declares exactly one authentication method in its own root document, WordPress application passwords, and that method gates only the write and privileged-read operations that are not part of the public surface.
kind: authentication
layout: security
method: probed
name: Energyx Authentication
name_suffix: Authentication
oauth_flows: []
overview: EnergyX declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: EnergyX
provider_slug: energyx
scheme_count: 0
schemes: []
slug: energyx-authentication
source_filename: energyx-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: probed\nsource: https://energyx.com/wp-json/\ndocs: https://developer.wordpress.org/rest-api/using-the-rest-api/authentication/\ndescription: >-\n  EnergyX publishes no developer program and issues no API credentials. The WordPress REST content\n  API behind energyx.com is anonymously readable — no key, token, signature or account is required\n  to read posts, pages, press releases, in-the-news coverage, leadership, job positions, partners,\n  videos, resource guides, media, taxonomies, search, the storefront catalog or the discovery\n  metadata. The server declares exactly one authentication method in its own root document,\n  WordPress application passwords, and that method gates only the write and privileged-read\n  operations that are not part of the public surface.\nsummary:\n  types: []\n  anonymous_read: true\n  credentialed_write: true\n  api_key_in: []\n  oauth2_flows: []\n  note: >-\n    No securityScheme appears in any of the fifteen\
  \ derived OpenAPI documents because the public\n    surface genuinely has none. This is a recorded absence, not a gap in harvesting. Running\n    0-working/derive-authentication.py against this repo returns zero schemes for the same reason.\nschemes: []\ndeclared_by_server:\n- name: application-passwords\n  type: http\n  scheme: basic\n  description: >-\n    WordPress application passwords (RFC 7617 Basic over TLS, username + generated application\n    password). Declared in the `authentication` block of the API root document. Required for every\n    write method and for privileged reads such as GET /wp/v2/settings. Credentials are issued per\n    WordPress user from the site admin — there is no public registration path, so this is a\n    staff-only credential, not a developer credential.\n  authorization_endpoint: https://energyx.com/wp/wp-admin/authorize-application.php\n  source: https://energyx.com/wp-json/\nadjacent_gated_surface:\n- namespace: wc/v3\n  description: >-\n    The WooCommerce\
  \ admin REST API is registered on the same host and would normally be reached\n    with a consumer key/secret pair. It returns 401 to an anonymous caller and there is no public\n    key issuance path, so it is out of scope and is deliberately not modelled in openapi/.\n  observed_status: 401\nevidence:\n- url: https://energyx.com/wp-json/\n  http_status: 200\n  finding: 'authentication: {\"application-passwords\": {\"endpoints\": {\"authorization\": \"https://energyx.com/wp/wp-admin/authorize-application.php\"}}}'\n- url: https://energyx.com/wp-json/wp/v2/posts?per_page=2\n  http_status: 200\n  finding: 'Anonymous read succeeds; response carries `Allow: GET`, confirming read-only anonymous access. X-WP-Total 69.'\n- url: https://energyx.com/wp-json/wp/v2/enx-press-release?per_page=1\n  http_status: 200\n  finding: Anonymous read of the site-specific press-release post type succeeds, X-WP-Total 39.\n- url: https://energyx.com/wp-json/wc/store/v1/products?per_page=1\n  http_status: 200\n\
  \  finding: Anonymous read of the WooCommerce Store API storefront catalog succeeds, X-WP-Total 15.\n- url: https://energyx.com/wp-json/wc/v3/products?per_page=1\n  http_status: 401\n  finding: WooCommerce admin API rejects the anonymous caller; no public credential path exists.\n- url: https://energyx.com/wp-json/wp/v2/settings\n  http_status: 401\n  finding: '{\"code\":\"rest_forbidden\",\"message\":\"Sorry, you are not allowed to do that.\",\"data\":{\"status\":401}}'\nx-evidence:\n  fetched: '2026-08-12'\n  probes: 6\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/energyx/refs/heads/main/authentication/energyx-authentication.yml
summary_line: 0 schemes
tags:
- Company
- Lithium
- Direct Lithium Extraction
- Critical Minerals
- Battery Technology
- Energy Transition
- Cleantech
- Materials Science
- Mining
- Chemicals
- Nuclear Materials
- Manufacturing
- Content
---
