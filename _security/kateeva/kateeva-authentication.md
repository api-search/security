---
api_key_in: []
api_specs:
- filename: kateeva-posts-api-openapi.yml
  format: yaml
  label: Kateeva Posts API
  slug: kateeva-posts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kateeva/refs/heads/main/openapi/kateeva-posts-api-openapi.yml
- filename: kateeva-pages-api-openapi.yml
  format: yaml
  label: Kateeva Pages API
  slug: kateeva-pages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kateeva/refs/heads/main/openapi/kateeva-pages-api-openapi.yml
- filename: kateeva-media-api-openapi.yml
  format: yaml
  label: Kateeva Media API
  slug: kateeva-media-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kateeva/refs/heads/main/openapi/kateeva-media-api-openapi.yml
- filename: kateeva-taxonomy-api-openapi.yml
  format: yaml
  label: Kateeva Taxonomy API
  slug: kateeva-taxonomy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kateeva/refs/heads/main/openapi/kateeva-taxonomy-api-openapi.yml
- filename: kateeva-search-api-openapi.yml
  format: yaml
  label: Kateeva Search API
  slug: kateeva-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kateeva/refs/heads/main/openapi/kateeva-search-api-openapi.yml
- filename: kateeva-discovery-api-openapi.yml
  format: yaml
  label: Kateeva Discovery API
  slug: kateeva-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kateeva/refs/heads/main/openapi/kateeva-discovery-api-openapi.yml
- filename: kateeva-oembed-api-openapi.yml
  format: yaml
  label: Kateeva oEmbed API
  slug: kateeva-oembed-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kateeva/refs/heads/main/openapi/kateeva-oembed-api-openapi.yml
- filename: kateeva-seo-api-openapi.yml
  format: yaml
  label: Kateeva SEO Metadata API
  slug: kateeva-seo-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kateeva/refs/heads/main/openapi/kateeva-seo-api-openapi.yml
auth_types: []
description: Kateeva publishes no developer program and issues no API credentials. The WordPress REST content API behind kateeva.com is anonymously readable — no key, token, signature or account is required to read posts, pages, media, taxonomies, search, oEmbed, SEO metadata or the discovery metadata. The server declares exactly one authentication method in its own root document, WordPress application passwords, and that method gates only the write and privileged-read operations that are not part of the public surface.
kind: authentication
layout: security
method: probed
name: Kateeva Authentication
name_suffix: Authentication
oauth_flows: []
overview: Kateeva declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: Kateeva
provider_slug: kateeva
scheme_count: 0
schemes: []
slug: kateeva-authentication
source_filename: kateeva-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-23'\nmethod: probed\nsource: https://kateeva.com/wp-json/\ndocs: https://developer.wordpress.org/rest-api/using-the-rest-api/authentication/\ndescription: >-\n  Kateeva publishes no developer program and issues no API credentials. The WordPress REST content\n  API behind kateeva.com is anonymously readable — no key, token, signature or account is required\n  to read posts, pages, media, taxonomies, search, oEmbed, SEO metadata or the discovery metadata.\n  The server declares exactly one authentication method in its own root document, WordPress\n  application passwords, and that method gates only the write and privileged-read operations that\n  are not part of the public surface.\nsummary:\n  types: []\n  anonymous_read: true\n  credentialed_write: true\n  api_key_in: []\n  oauth2_flows: []\n  note: >-\n    No securityScheme appears in any of the eight derived OpenAPI documents because the public\n    surface genuinely has none. This is a recorded absence,\
  \ not a gap in harvesting.\nschemes: []\ndeclared_by_server:\n- name: application-passwords\n  type: http\n  scheme: basic\n  description: >-\n    WordPress application passwords (RFC 7617 Basic over TLS, username + generated application\n    password). Declared in the `authentication` block of the API root document. Required for every\n    write method and for privileged reads such as GET /wp/v2/settings. Credentials are issued per\n    WordPress user from the site admin — there is no public registration path, so this is a\n    staff-only credential, not a developer credential.\n  authorization_endpoint: https://kateeva.com/wp-admin/authorize-application.php\n  source: https://kateeva.com/wp-json/\nevidence:\n- url: https://kateeva.com/wp-json/\n  http_status: 200\n  finding: 'authentication: {\"application-passwords\": {\"endpoints\": {\"authorization\": \"https://kateeva.com/wp-admin/authorize-application.php\"}}}'\n- url: https://kateeva.com/wp-json/wp/v2/posts?per_page=1\n  http_status:\
  \ 200\n  finding: 'Anonymous read succeeds; response carries `Allow: GET`, confirming read-only anonymous access. X-WP-Total 152.'\n- url: https://kateeva.com/wp-json/wp/v2/media?per_page=1\n  http_status: 200\n  finding: Anonymous read of the media library succeeds, X-WP-Total 236.\n- url: https://kateeva.com/wp-json/wp/v2/settings\n  http_status: 401\n  finding: '{\"code\":\"rest_forbidden\",\"message\":\"Sorry, you are not allowed to do that.\",\"data\":{\"status\":401}}'\n- url: https://kateeva.com/wp-json/contact-form-7/v1/contact-forms\n  http_status: 403\n  finding: The Contact Form 7 admin surface is credential-gated and is not part of the public read surface.\nx-evidence:\n  fetched: '2026-08-23'\n  probes: 5\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kateeva/refs/heads/main/authentication/kateeva-authentication.yml
summary_line: 0 schemes
tags:
- Company
- Display Manufacturing
- OLED
- Semiconductor Equipment
- Capital Equipment
- Inkjet Printing
- Thin Film Encapsulation
- Advanced Manufacturing
- Materials Deposition
- Consumer Electronics
- Hardware
- Content
---
