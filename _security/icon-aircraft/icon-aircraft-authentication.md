---
api_key_in: []
api_specs:
- filename: icon-aircraft-store-api-openapi.yml
  format: yaml
  label: Shop ICON Storefront API
  slug: icon-aircraft-store-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/icon-aircraft/refs/heads/main/openapi/icon-aircraft-store-api-openapi.yml
- filename: icon-aircraft-catalog-api-openapi.yml
  format: yaml
  label: ICON Aircraft Catalog API
  slug: icon-aircraft-catalog-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/icon-aircraft/refs/heads/main/openapi/icon-aircraft-catalog-api-openapi.yml
- filename: icon-aircraft-collections-api-openapi.yml
  format: yaml
  label: ICON Aircraft Collections API
  slug: icon-aircraft-collections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/icon-aircraft/refs/heads/main/openapi/icon-aircraft-collections-api-openapi.yml
- filename: icon-aircraft-discovery-api-openapi.yml
  format: yaml
  label: ICON Aircraft Discovery API
  slug: icon-aircraft-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/icon-aircraft/refs/heads/main/openapi/icon-aircraft-discovery-api-openapi.yml
- filename: icon-aircraft-media-api-openapi.yml
  format: yaml
  label: ICON Aircraft Media API
  slug: icon-aircraft-media-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/icon-aircraft/refs/heads/main/openapi/icon-aircraft-media-api-openapi.yml
- filename: icon-aircraft-pages-api-openapi.yml
  format: yaml
  label: ICON Aircraft Pages API
  slug: icon-aircraft-pages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/icon-aircraft/refs/heads/main/openapi/icon-aircraft-pages-api-openapi.yml
- filename: icon-aircraft-posts-api-openapi.yml
  format: yaml
  label: ICON Aircraft Posts API
  slug: icon-aircraft-posts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/icon-aircraft/refs/heads/main/openapi/icon-aircraft-posts-api-openapi.yml
- filename: icon-aircraft-search-api-openapi.yml
  format: yaml
  label: ICON Aircraft Search API
  slug: icon-aircraft-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/icon-aircraft/refs/heads/main/openapi/icon-aircraft-search-api-openapi.yml
- filename: icon-aircraft-taxonomy-api-openapi.yml
  format: yaml
  label: ICON Aircraft Taxonomy API
  slug: icon-aircraft-taxonomy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/icon-aircraft/refs/heads/main/openapi/icon-aircraft-taxonomy-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
method: probed
name: Icon Aircraft Authentication
name_suffix: Authentication
oauth_flows: []
overview: ICON Aircraft declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: ICON Aircraft
provider_slug: icon-aircraft
scheme_count: 0
schemes: []
slug: icon-aircraft-authentication
source_filename: icon-aircraft-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-22'\nmethod: probed\nsource: >-\n  Live anonymous probes of every surface in this profile plus the OAuth/OIDC discovery documents\n  saved under well-known/, 2026-08-22.\nsummary: >-\n  Every surface ICON Aircraft exposes is readable with no credentials at all. Neither OpenAPI in\n  this repo declares a securitySchemes block, because none of the described operations require one:\n  the WordPress content API, the Shopify storefront JSON endpoints and the UCP/MCP tools/list\n  method all answered 200 anonymously. Credentials appear only at two edges — WordPress application\n  passwords for writes on the corporate site, and Shopify customer-account OAuth/OIDC for a buyer's\n  own orders — and neither is a developer-program credential. There is no API key, no client\n  registration, and no way for a developer to obtain a token for ICON's own data.\nsurfaces:\n- surface: ICON Aircraft Content API\n  base: https://www.iconaircraft.com/wp-json\n  anonymous_read:\
  \ true\n  scheme: none\n  evidence:\n    probe: GET https://www.iconaircraft.com/wp-json/wp/v2/posts?per_page=1\n    status: 200\n  write_path:\n    scheme: http\n    type: basic\n    name: WordPress application passwords\n    authorization_endpoint: https://www.iconaircraft.com/wp-admin/authorize-application.php\n    note: >-\n      Declared in the `authentication` member of the /wp-json/ index document. This is the WordPress\n      admin credential path, not a published developer credential — there is no self-service signup\n      and no application registration. Every write method described by WordPress core on these\n      routes is out of reach for a third party.\n  gated_contexts:\n  - request: GET /wp/v2/settings\n    status: 401\n    code: rest_forbidden\n    note: context=edit and site settings require an authenticated administrator.\n- surface: Shop ICON Storefront API\n  base: https://store.iconaircraft.com\n  anonymous_read: true\n  scheme: none\n  evidence:\n    probe: GET\
  \ https://store.iconaircraft.com/products.json?limit=250\n    status: 200\n  note: >-\n    Session state on /cart.js is carried by Shopify session cookies (_shopify_essential, cart\n    token), not by a bearer credential. There is no storefront access token in this surface.\n- surface: Shop ICON UCP/MCP Server\n  base: https://store.iconaircraft.com/api/ucp/mcp\n  anonymous_read: true\n  scheme: none\n  evidence:\n    probe: POST /api/ucp/mcp {\"jsonrpc\":\"2.0\",\"id\":1,\"method\":\"tools/list\"}\n    status: 200\n    note: Returned 13 tools with full inputSchemas without any Authorization header.\n  agent_identity:\n    mechanism: >-\n      Every tool requires a `meta.ucp-agent.profile` URI in its arguments. This identifies the\n      calling agent to the merchant but is not authentication — it is not verified against a\n      registered client and grants no privilege.\n  protected_resource_metadata:\n    document: well-known/icon-aircraft-store-oauth-protected-resource.json\n    resource:\
  \ https://store.iconaircraft.com/api/ucp/mcp\n    authorization_servers:\n    - https://shopify.com/authentication/376732\n    bearer_methods_supported:\n    - header\n    rfc: RFC 9728\n    note: >-\n      The MCP endpoint advertises RFC 9728 protected-resource metadata even though tools/list\n      answered anonymously. Buyer-scoped operations (get_order, and payment on complete_checkout)\n      are where that authorization server is expected to be exercised.\n  authorization_server:\n    document: well-known/icon-aircraft-store-oauth-authorization-server.json\n    issuer: https://shopify.com/authentication/376732\n    rfc: RFC 8414\n  openid_connect:\n    document: well-known/icon-aircraft-store-openid-configuration.json\n    issuer: https://shopify.com/authentication/376732\n    note: >-\n      Shopify customer accounts. This authenticates a shopper to their own orders; it is not a\n      developer credential and issues no token for ICON Aircraft's own data.\nfindings:\n- id: no-developer-credential\n\
  \  severity: informational\n  detail: >-\n    There is no path by which a developer can obtain a credential for an ICON Aircraft API. Nothing\n    is gated because nothing is offered; the anonymous surfaces are the whole surface.\n- id: anonymous-author-records\n  severity: low\n  detail: >-\n    GET /wp-json/wp/v2/users returns 8 identifiable author records anonymously — a WordPress core\n    default, not a misconfiguration unique to ICON. It is documented here as an exposure and is\n    deliberately excluded from the derived OpenAPI, the agent skills and the MCP crosswalk. No\n    person's record is reproduced anywhere in this repository. Providers who want it closed can\n    filter the `users` REST endpoint for unauthenticated callers.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/icon-aircraft/refs/heads/main/authentication/icon-aircraft-authentication.yml
summary_line: 0 schemes
tags:
- Company
- Aerospace
- Aviation
- Aircraft Manufacturing
- Light Sport Aircraft
- Seaplanes
- General Aviation
- Flight Training
- Manufacturing
- Consumer Products
- E-Commerce
- Content
- Agentic Commerce
---
