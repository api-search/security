---
anonymous_access: false
api_key_in: []
auth_types: []
description: EnergyX publishes no developer program and issues no API credentials. The WordPress REST content API behind energyx.com is anonymously readable — no key, token, signature or account is required to read posts, pages, press releases, in-the-news coverage, leadership, job positions, partners, videos, resource guides, media, taxonomies, search, the storefront catalog or the discovery metadata. The server declares exactly one authentication method in its own root document, WordPress application passwords, and that method gates only the write and privileged-read operations that are not part of the public surface.
kind: authentication
layout: security
mechanism_count: 0
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
---
