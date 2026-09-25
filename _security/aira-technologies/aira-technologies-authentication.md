---
anonymous_access: false
api_key_in: []
auth_types: []
description: Aira Technologies publishes no developer program and issues no API credentials. The WordPress REST content API behind aira-technology.com is anonymously readable — no key, token, signature or account is required to read posts, pages, articles, events, media, categories, authors, search or the discovery metadata. The server declares exactly one authentication method in its own root document, WordPress application passwords, and that method gates only the write and privileged-read operations that are not part of the public surface. The Naavik and RANGPT products Aira actually sells have no public authentication surface at all — there is no developer portal, no signup, no key issuance and no documented token endpoint anywhere on the company's site.
kind: authentication
layout: security
mechanism_count: 0
method: probed
name: Aira Technologies Authentication
name_suffix: Authentication
oauth_flows: []
overview: Aira Technologies declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: Aira Technologies
provider_slug: aira-technologies
scheme_count: 0
schemes: []
slug: aira-technologies-authentication
source_filename: aira-technologies-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-14'\nmethod: probed\nsource: https://aira-technology.com/wp-json/\ndocs: https://developer.wordpress.org/rest-api/using-the-rest-api/authentication/\ndescription: >-\n  Aira Technologies publishes no developer program and issues no API credentials. The WordPress\n  REST content API behind aira-technology.com is anonymously readable — no key, token, signature\n  or account is required to read posts, pages, articles, events, media, categories, authors,\n  search or the discovery metadata. The server declares exactly one authentication method in its\n  own root document, WordPress application passwords, and that method gates only the write and\n  privileged-read operations that are not part of the public surface. The Naavik and RANGPT\n  products Aira actually sells have no public authentication surface at all — there is no\n  developer portal, no signup, no key issuance and no documented token endpoint anywhere on the\n  company's site.\nsummary:\n  types:\
  \ []\n  anonymous_read: true\n  credentialed_write: true\n  api_key_in: []\n  oauth2_flows: []\n  note: >-\n    No securityScheme appears in any of the ten derived OpenAPI documents because the public\n    surface genuinely has none. This is a recorded absence, not a gap in harvesting:\n    derive-authentication.py returned \"providers with auth profiles: 0\" against these specs.\nschemes: []\ndeclared_by_server:\n- name: application-passwords\n  type: http\n  scheme: basic\n  description: >-\n    WordPress application passwords (RFC 7617 Basic over TLS, username + generated application\n    password). Declared in the `authentication` block of the API root document. Required for every\n    write method and for privileged reads such as GET /wp/v2/settings and the WordPress Abilities\n    registry. Credentials are issued per WordPress user from the site admin — there is no public\n    registration path, so this is a staff-only credential, not a developer credential.\n  authorization_endpoint:\
  \ https://aira-technology.com/wp-admin/authorize-application.php\n  source: https://aira-technology.com/wp-json/\ngated_surfaces:\n- path: /wp/v2/settings\n  status: 401\n  finding: '{\"code\":\"rest_forbidden\",\"message\":\"Sorry, you are not allowed to do that.\",\"data\":{\"status\":401}}'\n- path: /wp-abilities/v1/abilities\n  status: 401\n  finding: >-\n    The WordPress Abilities registry — the site's agent-callable capability index — is registered\n    but returns 401 anonymously. If Aira ever opens it, this is the closest thing on the host to a\n    machine-discoverable tool surface; today it is auth-gated and its contents are unknown.\n- path: /wp-abilities/v1/categories\n  status: 401\n- path: /demos/\n  status: 200\n  finding: >-\n    Not an API surface, but the only other wall on the site: the product Demos page renders a\n    WordPress login form (\"You must be logged in to view this page\") rather than content.\nevidence:\n- url: https://aira-technology.com/wp-json/\n  http_status:\
  \ 200\n  finding: 'authentication: {\"application-passwords\": {\"endpoints\": {\"authorization\": \"https://aira-technology.com/wp-admin/authorize-application.php\"}}}'\n- url: https://aira-technology.com/wp-json/wp/v2/posts?per_page=2\n  http_status: 200\n  finding: 'Anonymous read succeeds; response carries `Allow: GET`, confirming read-only anonymous access.'\n- url: https://aira-technology.com/wp-json/wp/v2/article?per_page=1\n  http_status: 200\n  finding: Anonymous read of the site-specific `article` custom post type succeeds, X-WP-Total 3.\n- url: https://aira-technology.com/wp-json/wp/v2/settings\n  http_status: 401\n- url: https://aira-technology.com/wp-json/wp-abilities/v1/abilities\n  http_status: 401\nx-evidence:\n  fetched: '2026-09-14'\n  probes: 5\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aira-technologies/refs/heads/main/authentication/aira-technologies-authentication.yml
summary_line: 0 schemes
tags:
- Company
- Telecommunications
- Wireless
- Artificial Intelligence
- Machine Learning
- 5G
- Radio Access Network
- Network Automation
- Generative AI
- Observability
- Content
---
