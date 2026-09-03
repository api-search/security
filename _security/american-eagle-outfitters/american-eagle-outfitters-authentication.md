---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: probed
name: American Eagle Outfitters Authentication
name_suffix: Authentication
oauth_flows: []
overview: American Eagle Outfitters declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: American Eagle Outfitters
provider_slug: american-eagle-outfitters
scheme_count: 3
schemes:
- applies_to: https://www.unsubscribed.com/api/ucp/mcp
  description: The UCP shopping server identifies the calling agent by a profile URI rather than a bearer token. Discovery is anonymous; any invocation without a profile URI returns JSON-RPC error -32001 with data.code invalid_profile_url.
  evidence: 'Observed 2026-09-02: tools/list returned 200 with 13 tools; tools/call returned HTTP 422 / -32001 invalid_profile_url.'
  id: ucp_agent_profile
  location: JSON-RPC params.meta["ucp-agent"].profile
  not_required_for:
  - initialize
  - tools/list
  required_for:
  - tools/call
  - prompts/list
  - resources/list
  type: agent-identity
- applies_to: https://www.unsubscribed.com
  authorization_endpoint: https://account.unsubscribed.com/authentication/oauth/authorize
  description: Shopify customer-account OIDC for the Unsubscribed storefront. This authenticates a shopper, not a developer integration.
  end_session_endpoint: https://account.unsubscribed.com/authentication/logout
  id: shopify_customer_oidc
  id_token_signing_alg_values_supported:
  - RS256
  issuer: https://shopify.com/authentication/55041261720
  jwks_uri: https://account.unsubscribed.com/authentication/.well-known/jwks.json
  openid_configuration: https://www.unsubscribed.com/.well-known/openid-configuration
  response_types_supported:
  - code
  subject_types_supported:
  - public
  token_endpoint: https://account.unsubscribed.com/authentication/oauth/token
  token_endpoint_auth_methods_supported:
  - client_secret_basic
  - client_secret_post
  type: openIdConnect
- applies_to: https://www.unsubscribed.com
  authorization_servers:
  - https://account.unsubscribed.com
  - https://shopify.com/authentication/55041261720
  bearer_methods_supported:
  - header
  document: https://www.unsubscribed.com/.well-known/oauth-protected-resource
  id: shopify_protected_resource
  spec: RFC 9728 OAuth 2.0 Protected Resource Metadata
  type: oauth2
slug: american-eagle-outfitters-authentication
source_filename: american-eagle-outfitters-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-02'\nmethod: probed\nsource: https://www.unsubscribed.com/.well-known/openid-configuration\ndocs: https://www.unsubscribed.com/agents.md\nsummary: >-\n  American Eagle Outfitters publishes no developer authentication surface — there is no API\n  key programme, no developer portal and no documented auth page on www.ae.com or\n  www.aeo-inc.com. The only machine-readable auth metadata in the estate is served by\n  Shopify on the AEO brand storefront www.unsubscribed.com: a full OpenID Connect discovery\n  document and an RFC 9728 OAuth protected-resource document for customer accounts. The\n  UCP/MCP commerce endpoint itself takes no credential on discovery.\nschemes:\n- id: ucp_agent_profile\n  type: agent-identity\n  applies_to: https://www.unsubscribed.com/api/ucp/mcp\n  location: JSON-RPC params.meta[\"ucp-agent\"].profile\n  required_for:\n  - tools/call\n  - prompts/list\n  - resources/list\n  not_required_for:\n  - initialize\n  - tools/list\n  description:\
  \ >-\n    The UCP shopping server identifies the calling agent by a profile URI rather than a\n    bearer token. Discovery is anonymous; any invocation without a profile URI returns\n    JSON-RPC error -32001 with data.code invalid_profile_url.\n  evidence: 'Observed 2026-09-02: tools/list returned 200 with 13 tools; tools/call returned HTTP 422 / -32001 invalid_profile_url.'\n- id: shopify_customer_oidc\n  type: openIdConnect\n  applies_to: https://www.unsubscribed.com\n  openid_configuration: https://www.unsubscribed.com/.well-known/openid-configuration\n  issuer: https://shopify.com/authentication/55041261720\n  authorization_endpoint: https://account.unsubscribed.com/authentication/oauth/authorize\n  token_endpoint: https://account.unsubscribed.com/authentication/oauth/token\n  jwks_uri: https://account.unsubscribed.com/authentication/.well-known/jwks.json\n  end_session_endpoint: https://account.unsubscribed.com/authentication/logout\n  response_types_supported:\n  - code\n  token_endpoint_auth_methods_supported:\n\
  \  - client_secret_basic\n  - client_secret_post\n  id_token_signing_alg_values_supported:\n  - RS256\n  subject_types_supported:\n  - public\n  description: >-\n    Shopify customer-account OIDC for the Unsubscribed storefront. This authenticates a\n    shopper, not a developer integration.\n- id: shopify_protected_resource\n  type: oauth2\n  spec: RFC 9728 OAuth 2.0 Protected Resource Metadata\n  applies_to: https://www.unsubscribed.com\n  document: https://www.unsubscribed.com/.well-known/oauth-protected-resource\n  authorization_servers:\n  - https://account.unsubscribed.com\n  - https://shopify.com/authentication/55041261720\n  bearer_methods_supported:\n  - header\nhosts_with_no_auth_surface:\n- host: www.ae.com\n  note: /.well-known/openid-configuration and /.well-known/oauth-authorization-server both 404. No developer sign-up, no API key page.\n- host: www.aeo-inc.com\n  note: WordPress VIP corporate site. /wp-json/ advertises application-passwords for wp-admin only; all agent-facing\
  \ routes (wp-abilities/v1) return 401 rest_forbidden anonymously.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/american-eagle-outfitters/refs/heads/main/authentication/american-eagle-outfitters-authentication.yml
summary_line: 3 schemes
tags:
- Retail
- E-Commerce
- Fashion
- Apparel
- Consumer Goods
- Fortune 1000
---
