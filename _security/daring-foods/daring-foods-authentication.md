---
api_key_in: []
api_specs:
- filename: daring-foods-recipes-api-openapi.yml
  format: yaml
  label: Daring Foods Recipes API
  slug: daring-foods-recipes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/daring-foods/refs/heads/main/openapi/daring-foods-recipes-api-openapi.yml
- filename: daring-foods-products-api-openapi.yml
  format: yaml
  label: Daring Foods Retail Products API
  slug: daring-foods-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/daring-foods/refs/heads/main/openapi/daring-foods-products-api-openapi.yml
- filename: daring-foods-foodservice-api-openapi.yml
  format: yaml
  label: Daring Foods Foodservice Products API
  slug: daring-foods-foodservice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/daring-foods/refs/heads/main/openapi/daring-foods-foodservice-api-openapi.yml
- filename: daring-foods-pages-api-openapi.yml
  format: yaml
  label: Daring Foods Pages API
  slug: daring-foods-pages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/daring-foods/refs/heads/main/openapi/daring-foods-pages-api-openapi.yml
- filename: daring-foods-media-api-openapi.yml
  format: yaml
  label: Daring Foods Media API
  slug: daring-foods-media-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/daring-foods/refs/heads/main/openapi/daring-foods-media-api-openapi.yml
- filename: daring-foods-search-api-openapi.yml
  format: yaml
  label: Daring Foods Search API
  slug: daring-foods-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/daring-foods/refs/heads/main/openapi/daring-foods-search-api-openapi.yml
- filename: daring-foods-discovery-api-openapi.yml
  format: yaml
  label: Daring Foods Discovery API
  slug: daring-foods-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/daring-foods/refs/heads/main/openapi/daring-foods-discovery-api-openapi.yml
- filename: daring-foods-posts-api-openapi.yml
  format: yaml
  label: Daring Foods Posts API
  slug: daring-foods-posts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/daring-foods/refs/heads/main/openapi/daring-foods-posts-api-openapi.yml
- filename: daring-foods-oembed-api-openapi.yml
  format: yaml
  label: Daring Foods oEmbed API
  slug: daring-foods-oembed-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/daring-foods/refs/heads/main/openapi/daring-foods-oembed-api-openapi.yml
- filename: daring-foods-seo-api-openapi.yml
  format: yaml
  label: Daring Foods SEO Metadata API
  slug: daring-foods-seo-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/daring-foods/refs/heads/main/openapi/daring-foods-seo-api-openapi.yml
- filename: daring-foods-categories-api-openapi.yml
  format: yaml
  label: Daring Foods Categories API
  slug: daring-foods-categories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/daring-foods/refs/heads/main/openapi/daring-foods-categories-api-openapi.yml
- filename: daring-foods-comments-api-openapi.yml
  format: yaml
  label: Daring Foods Comments API
  slug: daring-foods-comments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/daring-foods/refs/heads/main/openapi/daring-foods-comments-api-openapi.yml
- filename: daring-foods-metadata-api-openapi.yml
  format: yaml
  label: Daring Foods Metadata API
  slug: daring-foods-metadata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/daring-foods/refs/heads/main/openapi/daring-foods-metadata-api-openapi.yml
- filename: daring-foods-tags-api-openapi.yml
  format: yaml
  label: Daring Foods Tags API
  slug: daring-foods-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/daring-foods/refs/heads/main/openapi/daring-foods-tags-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
method: probed
name: Daring Foods Authentication
name_suffix: Authentication
oauth_flows: []
overview: Daring Foods declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: Daring Foods
provider_slug: daring-foods
scheme_count: 0
schemes: []
slug: daring-foods-authentication
source_filename: daring-foods-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-04'\nmethod: probed\nsource: https://daring.com/wp-json/\ndocs: https://daring.com/wp-json/\nsummary:\n  types: []\n  api_key_in: []\n  oauth2_flows: []\n  public_read: true\n  credential_required_for_reads: false\nposture: >-\n  Every operation captured in openapi/ is anonymously readable - no API key, no token, no signup,\n  no rate-limit credential. That is not a design decision by Daring Foods; it is the WordPress core\n  default for public content, and it is why the derived OpenAPI documents declare no\n  securitySchemes (both derive-authentication.py and derive-oauth-scopes.py returned zero schemes\n  for this provider, which is the correct result rather than a gap).\nschemes: []\nwrite_side:\n  advertised: true\n  mechanism: WordPress Application Passwords\n  source: >-\n    The `authentication` block of the live route index at https://daring.com/wp-json/, which\n    returns:\n    {\"application-passwords\":{\"endpoints\":{\"authorization\":\"https://daring.com/wp-admin/authorize-application.php\"\
  }}}\n  authorization_endpoint: https://daring.com/wp-admin/authorize-application.php\n  note: >-\n    Application Passwords is the credential mechanism WordPress advertises for programmatic writes.\n    It is not obtainable by the public - it is issued from an authenticated wp-admin session on the\n    site - so it is recorded here as the documented write path, not as an onboarding route. Browser\n    sessions additionally use a cookie plus an X-WP-Nonce header, echoed in the\n    Access-Control-Allow-Headers response header observed on this host\n    (Authorization, X-WP-Nonce, Content-Disposition, Content-MD5, Content-Type).\nverified_behavior:\n- probe: GET /wp/v2/recipes?per_page=1\n  result: 200\n  note: Anonymous read succeeds.\n- probe: POST /wp/v2/recipes (no credentials)\n  result: 401\n  body: '{\"code\":\"rest_cannot_create\",\"message\":\"Sorry, you are not allowed to create posts as this user.\",\"data\":{\"status\":401}}'\n  note: Every write route rejects anonymous callers\
  \ with HTTP 401 and the WordPress error envelope.\n- probe: GET /wp/v2/settings\n  result: 401\n  note: Site settings require authentication and are deliberately excluded from the captured OpenAPI.\n- probe: GET /wp/v2/themes, /wp/v2/plugins, /wp/v2/block-types, /wp/v2/templates\n  result: 401\n  note: Administrative surfaces are credential-gated; not documented.\n- probe: GET /wp-abilities/v1/abilities\n  result: 401\n  body: '{\"code\":\"rest_forbidden\",\"message\":\"Sorry, you are not allowed to do that.\",\"data\":{\"status\":401}}'\n  note: >-\n    The WordPress Abilities API namespace is registered on this host but gated. Worth re-probing on\n    a later pass - it is the surface that would expose agent-callable abilities if the provider ever\n    opened it.\n- probe: 'GET /wp/v2/recipes?context=edit'\n  result: 401\n  note: Only the `view` and `embed` contexts are available anonymously.\ntransport:\n  https_only: true\n  tls_version: TLSv1.3\n  hsts: false\n  note: >-\n    No HSTS\
  \ header is served. See security/daring-foods-domain-security.yml for the full transport\n    and DNS posture.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/daring-foods/refs/heads/main/authentication/daring-foods-authentication.yml
summary_line: 0 schemes
tags:
- Company
- Food
- Consumer Packaged Goods
- Plant Based
- Alternative Protein
- Food and Beverage
- Recipes
- Foodservice
- Grocery
- Content
---
