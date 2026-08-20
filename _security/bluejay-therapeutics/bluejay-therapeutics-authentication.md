---
api_key_in: []
api_specs:
- filename: bluejay-therapeutics-content-api-openapi.yml
  format: yaml
  label: Bluejay Therapeutics Content API
  slug: bluejay-therapeutics-content-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bluejay-therapeutics/refs/heads/main/openapi/bluejay-therapeutics-content-api-openapi.yml
- filename: bluejay-therapeutics-discovery-api-openapi.yml
  format: yaml
  label: Bluejay Therapeutics Discovery API
  slug: bluejay-therapeutics-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bluejay-therapeutics/refs/heads/main/openapi/bluejay-therapeutics-discovery-api-openapi.yml
- filename: bluejay-therapeutics-embed-api-openapi.yml
  format: yaml
  label: Bluejay Therapeutics Embed API
  slug: bluejay-therapeutics-embed-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bluejay-therapeutics/refs/heads/main/openapi/bluejay-therapeutics-embed-api-openapi.yml
- filename: bluejay-therapeutics-empty-collections-api-openapi.yml
  format: yaml
  label: Bluejay Therapeutics Empty Collections API
  slug: bluejay-therapeutics-empty-collections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bluejay-therapeutics/refs/heads/main/openapi/bluejay-therapeutics-empty-collections-api-openapi.yml
- filename: bluejay-therapeutics-media-api-openapi.yml
  format: yaml
  label: Bluejay Therapeutics Media API
  slug: bluejay-therapeutics-media-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bluejay-therapeutics/refs/heads/main/openapi/bluejay-therapeutics-media-api-openapi.yml
- filename: bluejay-therapeutics-taxonomy-api-openapi.yml
  format: yaml
  label: Bluejay Therapeutics Taxonomy API
  slug: bluejay-therapeutics-taxonomy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bluejay-therapeutics/refs/heads/main/openapi/bluejay-therapeutics-taxonomy-api-openapi.yml
auth_types: []
description: 'The Bluejay Therapeutics Content API is the WordPress REST API behind bluejaytx.com. Its public read surface is entirely unauthenticated: posts, pages, media, categories, tags, search, types, taxonomies, statuses and the oEmbed provider all answer anonymously. Authentication exists only for the write and administrative surface, which is closed to the public.'
kind: authentication
layout: security
method: probed
name: Bluejay Therapeutics Authentication
name_suffix: Authentication
oauth_flows: []
overview: Bluejay Therapeutics declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Bluejay Therapeutics
provider_slug: bluejay-therapeutics
scheme_count: 1
schemes:
- applies_to: all 26 modelled read operations
  description: No credential is required or accepted for reads. Requests carrying no Authorization header return the same 200 responses as any other client.
  name: none
  sources:
  - openapi/bluejay-therapeutics-content-openapi.yml
  type: none
slug: bluejay-therapeutics-authentication
source_filename: bluejay-therapeutics-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-07'\nmethod: probed\nsource: https://bluejaytx.com/wp-json/\ndocs: https://developer.wordpress.org/rest-api/using-the-rest-api/authentication/\nsummary:\n  types: []\n  api_key_in: []\n  oauth2_flows: []\n  note: >-\n    The OpenAPI derived for this provider declares NO securitySchemes, and that is a faithful\n    record rather than a gap. Every one of the 26 modelled operations is a public read that\n    returns 200 without any credential, header or cookie. The mechanical\n    0-working/derive-authentication.py pass therefore produced no profile; this file was written\n    from the live probe instead.\nmodel: anonymous-read\ndescription: >-\n  The Bluejay Therapeutics Content API is the WordPress REST API behind bluejaytx.com. Its public\n  read surface is entirely unauthenticated: posts, pages, media, categories, tags, search, types,\n  taxonomies, statuses and the oEmbed provider all answer anonymously. Authentication exists only\n  for the write and\
  \ administrative surface, which is closed to the public.\nschemes:\n- name: none\n  type: none\n  applies_to: all 26 modelled read operations\n  description: >-\n    No credential is required or accepted for reads. Requests carrying no Authorization header\n    return the same 200 responses as any other client.\n  sources: [openapi/bluejay-therapeutics-content-openapi.yml]\nadvertised_mechanisms:\n- name: application-passwords\n  type: http\n  scheme: basic\n  description: >-\n    The site's own route index at /wp-json/ advertises exactly one authentication mechanism, under\n    the `authentication` key — WordPress Application Passwords, a per-user Basic credential issued\n    from wp-admin. This is the only way to reach the write and administrative routes.\n  authorization_endpoint: https://bluejaytx.com/wp-admin/authorize-application.php\n  public_issuance: false\n  note: >-\n    Issuance requires an existing wp-admin account, so this is a staff mechanism, not a developer\n    onboarding\
  \ path. There is no self-service signup, no key request form and no developer program.\n  source: https://bluejaytx.com/wp-json/\n- name: cookie-nonce\n  type: apiKey\n  in: header\n  parameter_name: X-WP-Nonce\n  description: >-\n    Standard WordPress logged-in cookie authentication paired with an X-WP-Nonce header, used by\n    the site's own admin JavaScript. The header is named in the Access-Control-Allow-Headers\n    response header on every route. Not usable by third parties.\n  source: response header Access-Control-Allow-Headers on https://bluejaytx.com/wp-json/wp/v2/posts\nauthorization:\n  model: WordPress capability checks\n  description: >-\n    Authorization is enforced per route by WordPress capability checks rather than by scopes.\n    Anonymous callers hold no capabilities, which is why the read surface is wide open and\n    everything else fails closed.\n  denied_anonymously:\n  - {route: /wp/v2/settings, status: 401, code: rest_forbidden}\n  - {route: /wp/v2/themes,\
  \ status: 401, code: rest_cannot_view_themes}\n  - {route: /wp/v2/plugins, status: 401, code: rest_cannot_view_plugins}\n  - {route: /wp/v2/menus, status: 401, code: rest_cannot_view}\n  - {route: /wp/v2/menu-locations, status: 401, code: rest_cannot_view}\n  - {route: /wp/v2/widgets, status: 401, code: rest_cannot_manage_widgets}\n  - {route: /wp/v2/block-types, status: 401, code: rest_block_type_cannot_view}\n  - {route: /wp/v2/templates, status: 401, code: rest_cannot_manage_templates}\n  - {route: /wp/v2/font-collections, status: 401, code: rest_cannot_read}\n  - {route: /wp/v2/icons, status: 401, code: rest_cannot_view}\n  - {route: /wp-abilities/v1/abilities, status: 401, code: rest_forbidden}\n  - {route: /wp-abilities/v1/categories, status: 401, code: rest_forbidden}\n  - {route: /oembed/1.0/proxy, status: 401, code: rest_forbidden}\n  - {route: /aioseo/v1/ping, status: 401, code: rest_forbidden}\n  - {route: /aioseo/v1/options, status: 401, code: rest_forbidden}\n  - {route: /elementor/v1/globals,\
  \ status: 401, code: rest_forbidden}\n  - {route: /wp-site-health/v1/tests/background-updates, status: 401, code: rest_forbidden}\n  - {route: /contact-form-7/v1/contact-forms, status: 403, code: wpcf7_forbidden}\n  writes_denied: >-\n    Every POST/PUT/PATCH/DELETE endpoint in the route index is capability-gated. No write was\n    attempted during this pass; the read-side 401s above are the evidence that anonymous callers\n    hold no capabilities.\nrate_limiting:\n  documented: false\n  observed_headers: []\n  note: >-\n    No RateLimit, X-RateLimit-* or Retry-After headers were observed on any anonymous response.\n    The site is fronted by WP Engine (nginx) and its robots.txt requests a 10-second crawl delay,\n    which is the only throttling signal the provider publishes.\nx-evidence:\n  fetched: '2026-08-07'\n  url: https://bluejaytx.com/wp-json/\n  http_status: 200\n  content_type: application/json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bluejay-therapeutics/refs/heads/main/authentication/bluejay-therapeutics-authentication.yml
summary_line: 1 scheme
tags:
- Company
- biopharmaceuticals
- Pharmaceuticals
- Life Sciences
- hepatology
- Infectious Disease
- Clinical Trials
- Drug Development
- Monoclonal Antibodies
- content-api
---
