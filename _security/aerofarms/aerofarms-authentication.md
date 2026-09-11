---
anonymous_access: false
api_key_in: []
api_specs:
- filename: aerofarms-news-openapi.yml
  format: yaml
  label: AeroFarms News API
  slug: aerofarms-news-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aerofarms/refs/heads/main/openapi/aerofarms-news-openapi.yml
- filename: aerofarms-pages-openapi.yml
  format: yaml
  label: AeroFarms Pages API
  slug: aerofarms-pages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aerofarms/refs/heads/main/openapi/aerofarms-pages-openapi.yml
- filename: aerofarms-products-openapi.yml
  format: yaml
  label: AeroFarms Products API
  slug: aerofarms-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aerofarms/refs/heads/main/openapi/aerofarms-products-openapi.yml
- filename: aerofarms-store-openapi.yml
  format: yaml
  label: AeroFarms Store API
  slug: aerofarms-store-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aerofarms/refs/heads/main/openapi/aerofarms-store-openapi.yml
- filename: aerofarms-faq-openapi.yml
  format: yaml
  label: AeroFarms FAQ API
  slug: aerofarms-faq-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aerofarms/refs/heads/main/openapi/aerofarms-faq-openapi.yml
- filename: aerofarms-taxonomy-openapi.yml
  format: yaml
  label: AeroFarms Taxonomy API
  slug: aerofarms-taxonomy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aerofarms/refs/heads/main/openapi/aerofarms-taxonomy-openapi.yml
- filename: aerofarms-media-openapi.yml
  format: yaml
  label: AeroFarms Media API
  slug: aerofarms-media-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aerofarms/refs/heads/main/openapi/aerofarms-media-openapi.yml
- filename: aerofarms-search-openapi.yml
  format: yaml
  label: AeroFarms Search API
  slug: aerofarms-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aerofarms/refs/heads/main/openapi/aerofarms-search-openapi.yml
- filename: aerofarms-discovery-openapi.yml
  format: yaml
  label: AeroFarms Discovery API
  slug: aerofarms-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aerofarms/refs/heads/main/openapi/aerofarms-discovery-openapi.yml
auth_types: []
description: 'AeroFarms publishes no authentication documentation, because it publishes no developer program. Everything here was established by calling the surface and reading the two OAuth discovery documents the site really serves. The surface splits cleanly in three: an anonymous read tier that needs no credential at all, an OAuth 2.1 tier that guards the MCP server, and an ordinary WordPress session tier that guards everything else.'
kind: authentication
layout: security
mechanism_count: 0
method: probed
name: Aerofarms Authentication
name_suffix: Authentication
oauth_flows: []
overview: AeroFarms declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: AeroFarms
provider_slug: aerofarms
scheme_count: 0
schemes: []
slug: aerofarms-authentication
source_filename: aerofarms-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-10'\nmethod: probed\nsource: >-\n  Live probes of https://www.aerofarms.com/wp-json/* on 2026-09-10, plus the provider-served\n  /.well-known/oauth-authorization-server and /.well-known/oauth-protected-resource documents.\ndescription: >-\n  AeroFarms publishes no authentication documentation, because it publishes no developer program.\n  Everything here was established by calling the surface and reading the two OAuth discovery\n  documents the site really serves. The surface splits cleanly in three: an anonymous read tier that\n  needs no credential at all, an OAuth 2.1 tier that guards the MCP server, and an ordinary WordPress\n  session tier that guards everything else.\n\ntiers:\n\n- name: anonymous-read\n  applies_to: >-\n    wp/v2 posts, pages, product, product_cat, categories, tags, ufaq, ufaq-category, media, search,\n    comments, types, taxonomies, statuses; wc/store/v1 products, product categories, collection-data\n    and cart; the wp-json route\
  \ index.\n  credential: none\n  verified: >-\n    Every route above returned HTTP 200 with real data on 2026-09-10 with no Authorization header and\n    no cookie. The product collection answers `Allow: GET` and returns X-WP-Total.\n  write_access: >-\n    None. POST/PUT/DELETE are registered on many of these routes but every one of them is capability\n    gated; an anonymous caller gets 401 rest_forbidden. The public contract is read-only.\n\n- name: oauth2-mcp\n  applies_to: https://www.aerofarms.com/wp-json/mcp/mcp-oauth-server\n  credential: OAuth 2.1 bearer token, scope `mcp`\n  discovery:\n    protected_resource: https://www.aerofarms.com/.well-known/oauth-protected-resource\n    authorization_server: https://www.aerofarms.com/.well-known/oauth-authorization-server\n    challenge: >-\n      WWW-Authenticate: Bearer realm=\"https://www.aerofarms.com\",\n      resource_metadata=\"https://www.aerofarms.com/.well-known/oauth-protected-resource\"\n  issuer: https://www.aerofarms.com\n\
  \  authorization_endpoint: https://www.aerofarms.com/oauth/authorize\n  token_endpoint: https://www.aerofarms.com/oauth/token\n  revocation_endpoint: https://www.aerofarms.com/oauth/revoke\n  response_types: [code]\n  grant_types: [authorization_code, refresh_token]\n  pkce: S256\n  pkce_required: true\n  token_endpoint_auth_methods: [none]\n  client_registration: >-\n    No dynamic client registration endpoint. The server advertises\n    client_id_metadata_document_supported: true, i.e. a client identifies itself with a URL that\n    resolves to its own client metadata document.\n  bearer_methods: [header]\n  scopes: [mcp]\n  see: scopes/aerofarms-scopes.yml\n  verified: >-\n    Probed 2026-09-10: an anonymous JSON-RPC tools/list returned HTTP 401 with the challenge above and\n    body {\"code\":\"mcp_unauthorized\"}. No token was obtained and none was attempted — this profile is\n    built entirely from anonymous requests.\n\n- name: wordpress-session\n  applies_to: >-\n    Every write\
  \ method on wp/v2 and wc/store; the whole of wc/v3, wc-admin, wc-analytics,\n    wp-abilities/v1, wp/v2/users, and /wp-json/mcp/mcp-adapter-default-server.\n  credential: >-\n    WordPress cookie + X-WP-Nonce for first-party browser calls, or an application password over HTTP\n    Basic for programmatic calls. Neither is issuable by a member of the public — there is no signup.\n  verified: >-\n    wc/v3/products returned 401 woocommerce_rest_cannot_view; wp/v2/users returned 401\n    rest_user_cannot_view; wp-abilities/v1/abilities and mcp-adapter-default-server returned 401\n    rest_forbidden. The Store API advertises the browser scheme in its CORS preflight:\n    Access-Control-Allow-Headers includes Authorization, X-WP-Nonce, Cart-Token and Nonce.\n\nsignup:\n  available: false\n  note: >-\n    AeroFarms operates no developer signup, no API key issuance and no partner portal. An agent can\n    read the public tier today and can negotiate OAuth against the MCP server only if it already\
  \ has\n    a WordPress identity on this site.\n\nsecurity_schemes_in_spec:\n  present: false\n  note: >-\n    The derived OpenAPI documents in openapi/ describe only the anonymous read tier, so they declare\n    no securitySchemes. That is faithful to the surface rather than an omission: adding a scheme the\n    public caller never uses would misdescribe the contract.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aerofarms/refs/heads/main/authentication/aerofarms-authentication.yml
summary_line: 0 schemes
tags:
- Company
- Agriculture
- Vertical Farming
- Indoor Farming
- AgTech
- Food and Beverage
- Consumer Packaged Goods
- Microgreens
- Sustainability
- Content
- Commerce
- MCP
---
