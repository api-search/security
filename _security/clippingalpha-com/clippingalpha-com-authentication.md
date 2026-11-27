---
anonymous_access: true
api_key_in: []
auth_types:
- none
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: probed
name: ClippingAlpha Authentication
name_suffix: Authentication
oauth_flows: []
overview: ClippingAlpha secures its APIs with none and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: ClippingAlpha
provider_slug: clippingalpha-com
scheme_count: 2
schemes:
- applies_to:
  - search_campaigns
  - get_campaign
  - top_alpha_now
  - board_summary
  - get_brief
  - get_moments
  - get_assets
  - plan_clips
  - get_campaign_analytics
  - compare_campaigns
  - show_campaign
  - browse_campaigns
  description: '"Auth: none for the campaign tools." 12 of the 23 MCP tools answer signed out (README).'
  name: anonymous
  type: none
- applies_to:
  - my_saved_campaigns
  - save_campaign
  - my_alert_rules
  - set_alert_rule
  - delete_alert_rule
  - my_referral
  - cut_clips
  - my_clips
  - connect_account
  - check_account
  - my_accounts
  authorization_response_iss_parameter_supported: true
  client_id_metadata_document_supported: false
  code_challenge_methods_supported:
  - S256
  description: '"OAuth with dynamic client registration for the account tools." Authorization code with PKCE (S256), public clients (token_endpoint_auth_methods_supported: none), refresh tokens, RFC 9728 protected-resource metadata pointing at issuer https://clippingalpha.com.'
  flows:
    authorizationCode:
      authorizationUrl: https://clippingalpha.com/app/connect
      refreshUrl: https://clippingalpha.com/api/oauth/token
      scopes:
        clipper: Sign-in scope for the signed-in clipper's account tools (only scope advertised).
      tokenUrl: https://clippingalpha.com/api/oauth/token
  grant_types_supported:
  - authorization_code
  - refresh_token
  name: clippingalphaOAuth
  registration_endpoint: https://clippingalpha.com/api/oauth/register
  revocation_endpoint: https://clippingalpha.com/api/oauth/revoke
  type: oauth2
slug: clippingalpha-com-authentication
source_filename: clippingalpha-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: probed\nsource: https://clippingalpha.com/.well-known/oauth-authorization-server (HTTP 200), https://clippingalpha.com/.well-known/oauth-protected-resource/mcp (HTTP 200), https://github.com/ClippingAlpha/clippingalpha-mcp/blob/main/README.md\ndocs: https://clippingalpha.com/learn/clippingalpha-mcp-setup\nsummary:\n  types:\n  - none\n  - oauth2\n  note: No OpenAPI is published; the profile is read from the MCP server's published OAuth metadata documents and its docs. Token, registration and revocation endpoints were read from metadata only and never called.\nschemes:\n- name: anonymous\n  type: none\n  description: '\"Auth: none for the campaign tools.\" 12 of the 23 MCP tools answer signed out (README).'\n  applies_to: [search_campaigns, get_campaign, top_alpha_now, board_summary, get_brief, get_moments, get_assets, plan_clips, get_campaign_analytics, compare_campaigns, show_campaign, browse_campaigns]\n- name: clippingalphaOAuth\n  type:\
  \ oauth2\n  description: '\"OAuth with dynamic client registration for the account tools.\" Authorization code with PKCE (S256), public clients (token_endpoint_auth_methods_supported: none), refresh tokens, RFC 9728 protected-resource metadata pointing at issuer https://clippingalpha.com.'\n  flows:\n    authorizationCode:\n      authorizationUrl: https://clippingalpha.com/app/connect\n      tokenUrl: https://clippingalpha.com/api/oauth/token\n      refreshUrl: https://clippingalpha.com/api/oauth/token\n      scopes:\n        clipper: Sign-in scope for the signed-in clipper's account tools (only scope advertised).\n  registration_endpoint: https://clippingalpha.com/api/oauth/register\n  revocation_endpoint: https://clippingalpha.com/api/oauth/revoke\n  code_challenge_methods_supported: [S256]\n  grant_types_supported: [authorization_code, refresh_token]\n  authorization_response_iss_parameter_supported: true\n  client_id_metadata_document_supported: false\n  applies_to: [my_saved_campaigns,\
  \ save_campaign, my_alert_rules, set_alert_rule, delete_alert_rule, my_referral, cut_clips, my_clips, connect_account, check_account, my_accounts]\n"
source_yaml_url: https://artifacts.apis.io/clippingalpha-com/authentication/clippingalpha-com-authentication.yml
summary_line: none/oauth2 · 2 schemes
tags:
- Company
- Clipping
- UGC
- Creator Economy
- Influencer Marketing
- Campaigns
- MCP
- Open Data
- Short-Form Video
---
