---
api_key_in:
- query
- body
auth_types:
- none
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Vidjet Authentication
name_suffix: Authentication
oauth_flows: []
overview: Vidjet secures its APIs with none and apiKey across 4 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Vidjet
provider_slug: vidjet
scheme_count: 4
schemes:
- applies_to:
  - GET /widgets
  evidence: GET https://app-api.vidjet.io/widgets returned HTTP 200 with application/json and no credential of any kind on 2026-08-13. With no siteId it returned a default test site record; with an unknown siteId it returned 200 and an empty site object. Read access to the campaign-resolution endpoint is anonymous by design — it is called from the browser by the embed script.
  name: none
  type: none
- evidence: The documented embed snippet is media.vidjet.io/client-app.js?siteId=xxxxxxxx-xxxx-xxxx-xxxx-xxxxxxxxxxxx and the script forwards it as GET ${backend}/widgets?siteId=... . It is a public tenant identifier shipped in page source, not a credential.
  format: UUID v4
  in: query
  name: siteId
  note: Because it is embedded in every customer's HTML, siteId must be treated as public. It selects a tenant; it does not authorize anything.
  parameter: siteId
  secret: false
  type: apiKey
- evidence: Vidjet_Api::install() POSTs to /plugins/install and, on HTTP 200, stores `siteId` and `authToken` from the response via Vidjet_Settings::set_settings(); the plugin persists them in a WordPress option. The pair is also accepted on the way in as body.integrationKeys.{siteId,authToken} when re-installing.
  in: body
  issued_by: POST https://app-api.vidjet.io/plugins/install
  name: authToken
  parameter: integrationKeys.authToken
  rotation: not documented
  scopes: none published
  secret: true
  type: apiKey
- applies_to:
  - POST /woocommerce/auth-callback
  evidence: 'The plugin registers https://app-api.vidjet.io/woocommerce/auth-callback as the return endpoint of the WooCommerce REST API key-generation flow, so Vidjet receives WooCommerce consumer credentials for the merchant store. OPTIONS on that path returned 200 with `Allow: POST`.'
  name: woocommerce-auth-callback
  note: This is WooCommerce's authorization handshake, not a Vidjet OAuth server. Vidjet publishes no authorization or token endpoint of its own — every /.well-known/oauth-authorization-server and /.well-known/openid-configuration probe on every Vidjet host returned 404 or 403.
  type: oauth-like-handshake
slug: vidjet-authentication
source_filename: vidjet-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: derived\nsource: >-\n  wordpress.org/plugins/vidjet (includes/class-vidjet-api.php,\n  includes/class-vidjet-settings.php, v1.1.4) + media.vidjet.io/client-app.js +\n  live unauthenticated probes of app-api.vidjet.io on 2026-08-13\nnote: >-\n  Vidjet publishes no authentication documentation. There is no OpenAPI to derive\n  securitySchemes from, so this profile is derived from the two first-party\n  artifacts Vidjet does publish (the GPL WordPress plugin source and the public\n  embed script) plus what the live API returned to anonymous requests. Nothing\n  here is inferred from naming or convention.\ndocs: null\nsummary:\n  types: [none, apiKey]\n  documented_by_provider: false\n  oauth2: false\n  openid_connect: false\n  mutual_tls: false\n  api_key_in: [query, body]\nschemes:\n- name: none\n  type: none\n  applies_to:\n  - GET /widgets\n  evidence: >-\n    GET https://app-api.vidjet.io/widgets returned HTTP 200 with\n    application/json\
  \ and no credential of any kind on 2026-08-13. With no siteId\n    it returned a default test site record; with an unknown siteId it returned\n    200 and an empty site object. Read access to the campaign-resolution endpoint\n    is anonymous by design — it is called from the browser by the embed script.\n- name: siteId\n  type: apiKey\n  in: query\n  parameter: siteId\n  format: UUID v4\n  secret: false\n  evidence: >-\n    The documented embed snippet is\n    media.vidjet.io/client-app.js?siteId=xxxxxxxx-xxxx-xxxx-xxxx-xxxxxxxxxxxx and\n    the script forwards it as GET ${backend}/widgets?siteId=... . It is a public\n    tenant identifier shipped in page source, not a credential.\n  note: >-\n    Because it is embedded in every customer's HTML, siteId must be treated as\n    public. It selects a tenant; it does not authorize anything.\n- name: authToken\n  type: apiKey\n  in: body\n  parameter: integrationKeys.authToken\n  secret: true\n  evidence: >-\n    Vidjet_Api::install() POSTs\
  \ to /plugins/install and, on HTTP 200, stores\n    `siteId` and `authToken` from the response via\n    Vidjet_Settings::set_settings(); the plugin persists them in a WordPress\n    option. The pair is also accepted on the way in as\n    body.integrationKeys.{siteId,authToken} when re-installing.\n  issued_by: POST https://app-api.vidjet.io/plugins/install\n  rotation: not documented\n  scopes: none published\n- name: woocommerce-auth-callback\n  type: oauth-like-handshake\n  applies_to:\n  - POST /woocommerce/auth-callback\n  evidence: >-\n    The plugin registers https://app-api.vidjet.io/woocommerce/auth-callback as\n    the return endpoint of the WooCommerce REST API key-generation flow, so\n    Vidjet receives WooCommerce consumer credentials for the merchant store.\n    OPTIONS on that path returned 200 with `Allow: POST`.\n  note: >-\n    This is WooCommerce's authorization handshake, not a Vidjet OAuth server.\n    Vidjet publishes no authorization or token endpoint of its own\
  \ — every\n    /.well-known/oauth-authorization-server and /.well-known/openid-configuration\n    probe on every Vidjet host returned 404 or 403.\ntransport:\n  https_only: true\n  observed_headers:\n    access-control-allow-origin: '*'\n    access-control-allow-methods: PUT, POST, GET, DELETE, OPTIONS\n    access-control-allow-headers: Origin, X-Requested-With, Content-Type, Accept\n  note: >-\n    CORS is fully open on app-api.vidjet.io, consistent with an API designed to be\n    called from arbitrary merchant storefronts.\ngaps:\n- No published authentication documentation of any kind.\n- No documented way for a merchant to obtain an API credential outside of installing a platform plugin.\n- No scopes, no token expiry, no rotation or revocation policy published.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vidjet/refs/heads/main/authentication/vidjet-authentication.yml
summary_line: none/apiKey · 4 schemes
tags:
- Company
- E-Commerce
- Video
- Shoppable Video
- Shopify
- Conversion
- Marketing
- No-code
- Widgets
- Embed
---
