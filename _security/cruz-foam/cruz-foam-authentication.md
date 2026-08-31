---
api_key_in: []
api_specs:
- filename: cruz-foam-posts-api-openapi.yml
  format: yaml
  label: Cruz Foam Posts API
  slug: cruz-foam-posts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cruz-foam/refs/heads/main/openapi/cruz-foam-posts-api-openapi.yml
- filename: cruz-foam-pages-api-openapi.yml
  format: yaml
  label: Cruz Foam Pages API
  slug: cruz-foam-pages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cruz-foam/refs/heads/main/openapi/cruz-foam-pages-api-openapi.yml
- filename: cruz-foam-customers-api-openapi.yml
  format: yaml
  label: Cruz Foam Customers API
  slug: cruz-foam-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cruz-foam/refs/heads/main/openapi/cruz-foam-customers-api-openapi.yml
- filename: cruz-foam-media-api-openapi.yml
  format: yaml
  label: Cruz Foam Media API
  slug: cruz-foam-media-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cruz-foam/refs/heads/main/openapi/cruz-foam-media-api-openapi.yml
- filename: cruz-foam-search-api-openapi.yml
  format: yaml
  label: Cruz Foam Search API
  slug: cruz-foam-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cruz-foam/refs/heads/main/openapi/cruz-foam-search-api-openapi.yml
- filename: cruz-foam-discovery-api-openapi.yml
  format: yaml
  label: Cruz Foam Discovery API
  slug: cruz-foam-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cruz-foam/refs/heads/main/openapi/cruz-foam-discovery-api-openapi.yml
- filename: cruz-foam-oembed-api-openapi.yml
  format: yaml
  label: Cruz Foam oEmbed API
  slug: cruz-foam-oembed-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cruz-foam/refs/heads/main/openapi/cruz-foam-oembed-api-openapi.yml
- filename: cruz-foam-seo-api-openapi.yml
  format: yaml
  label: Cruz Foam SEO Metadata API
  slug: cruz-foam-seo-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cruz-foam/refs/heads/main/openapi/cruz-foam-seo-api-openapi.yml
- filename: cruz-foam-categories-api-openapi.yml
  format: yaml
  label: Cruz Foam Categories API
  slug: cruz-foam-categories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cruz-foam/refs/heads/main/openapi/cruz-foam-categories-api-openapi.yml
- filename: cruz-foam-portfolio-categories-api-openapi.yml
  format: yaml
  label: Cruz Foam Portfolio Categories API
  slug: cruz-foam-portfolio-categories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cruz-foam/refs/heads/main/openapi/cruz-foam-portfolio-categories-api-openapi.yml
- filename: cruz-foam-tags-api-openapi.yml
  format: yaml
  label: Cruz Foam Tags API
  slug: cruz-foam-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cruz-foam/refs/heads/main/openapi/cruz-foam-tags-api-openapi.yml
- filename: cruz-foam-users-api-openapi.yml
  format: yaml
  label: Cruz Foam Users API
  slug: cruz-foam-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cruz-foam/refs/heads/main/openapi/cruz-foam-users-api-openapi.yml
auth_types: []
description: Cruz Foam publishes no developer program and issues no API credentials. The WordPress REST content API behind cruzfoam.com is anonymously readable — no key, token, signature or account is required to read posts, pages, the customer showcase, media, taxonomies, search or the discovery metadata. The server declares exactly one authentication method in its own root document, WordPress application passwords, and that method gates only the write and privileged-read operations that are not part of the public surface.
kind: authentication
layout: security
method: probed
name: Cruz Foam Authentication
name_suffix: Authentication
oauth_flows: []
overview: Cruz Foam declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: Cruz Foam
provider_slug: cruz-foam
scheme_count: 0
schemes: []
slug: cruz-foam-authentication
source_filename: cruz-foam-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-11'\nmethod: probed\nsource: https://cruzfoam.com/wp-json/\ndocs: https://developer.wordpress.org/rest-api/using-the-rest-api/authentication/\ndescription: >-\n  Cruz Foam publishes no developer program and issues no API credentials. The WordPress REST\n  content API behind cruzfoam.com is anonymously readable — no key, token, signature or account is\n  required to read posts, pages, the customer showcase, media, taxonomies, search or the discovery\n  metadata. The server declares exactly one authentication method in its own root document,\n  WordPress application passwords, and that method gates only the write and privileged-read\n  operations that are not part of the public surface.\nsummary:\n  types: []\n  anonymous_read: true\n  credentialed_write: true\n  api_key_in: []\n  oauth2_flows: []\n  note: >-\n    No securityScheme appears in any of the nine derived OpenAPI documents because the public\n    surface genuinely has none. This is a recorded absence,\
  \ not a gap in harvesting.\nschemes: []\ndeclared_by_server:\n  - name: application-passwords\n    type: http\n    scheme: basic\n    description: >-\n      WordPress application passwords (RFC 7617 Basic over TLS, username + generated\n      application password). Declared in the `authentication` block of the API root document.\n      Required for every write method and for privileged reads such as GET /wp/v2/settings.\n      Credentials are issued per WordPress user from the site admin — there is no public\n      registration path, so this is a staff-only credential, not a developer credential.\n    authorization_endpoint: https://cruzfoam.com/wp-admin/authorize-application.php\n    source: https://cruzfoam.com/wp-json/\nevidence:\n  - url: https://cruzfoam.com/wp-json/\n    http_status: 200\n    finding: 'authentication: {\"application-passwords\": {\"endpoints\": {\"authorization\": \"https://cruzfoam.com/wp-admin/authorize-application.php\"}}}'\n  - url: https://cruzfoam.com/wp-json/wp/v2/posts?per_page=1\n\
  \    http_status: 200\n    finding: 'Anonymous read succeeds; response carries `Allow: GET`, confirming read-only anonymous access.'\n  - url: https://cruzfoam.com/wp-json/wp/v2/customers?per_page=1\n    http_status: 200\n    finding: Anonymous read of the site-specific customers post type succeeds, X-WP-Total 20.\n  - url: https://cruzfoam.com/wp-json/wp/v2/settings\n    http_status: 401\n    finding: '{\"code\":\"rest_forbidden\",\"message\":\"Sorry, you are not allowed to do that.\",\"data\":{\"status\":401}}'\nx-evidence:\n  fetched: '2026-08-11'\n  probes: 4\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cruz-foam/refs/heads/main/authentication/cruz-foam-authentication.yml
summary_line: 0 schemes
tags:
- Company
- Materials Science
- Sustainable Packaging
- Compostable Materials
- Biomaterials
- Circular Economy
- Manufacturing
- Consumer Packaged Goods
- Cold Chain
- Sustainability
- Content
---
