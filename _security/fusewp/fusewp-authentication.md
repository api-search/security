---
api_key_in:
- admin-form
auth_types:
- oauth2
- apiKey
description: ''
kind: authentication
layout: security
method: probed
name: Fusewp Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- refreshToken
overview: FuseWP secures its APIs with oauth2 and apiKey across 0 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and refreshToken flow(s).
provider_name: FuseWP
provider_slug: fusewp
scheme_count: 0
schemes: []
slug: fusewp-authentication
source_filename: fusewp-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: probed\nsource: https://auth.fusewp.com/\ndocs: https://fusewp.com/article/installation-activation/\nnote: >-\n  FuseWP publishes no OpenAPI, so no securityScheme could be derived\n  mechanically. This profile was assembled from two real sources: the\n  GPL-licensed first-party plugin source shipped at\n  https://downloads.wordpress.org/plugin/fusewp.1.1.26.1.zip (specifically\n  src/core/src/Integrations/AbstractIntegration.php and\n  src/core/src/Base.php), and live HTTP probes of auth.fusewp.com and\n  fusewp.com on 2026-08-12. Nothing here is inferred from marketing copy.\nsummary:\n  types: [oauth2, apiKey]\n  api_key_in: [admin-form]\n  oauth2_flows: [authorizationCode, refreshToken]\n  surfaces: 3\nsurfaces:\n- id: oauth-broker\n  name: FuseWP OAuth Broker\n  host: https://auth.fusewp.com\n  type: oauth2\n  role: >-\n    Confidential-client proxy. The FuseWP plugin runs self-hosted on the\n    customer's server and therefore cannot hold\
  \ OAuth client secrets for the\n    partner platforms. FuseWP registers ONE OAuth application per partner\n    against its own auth.fusewp.com redirect URI and brokers the code exchange\n    and refresh on the customer's behalf.\n  flows:\n  - flow: authorizationCode\n    initiation: GET https://auth.fusewp.com/{integration_id}\n    parameters:\n    - name: fwpnonce\n      in: query\n      required: true\n      description: >-\n        WordPress nonce minted by the plugin as wp_create_nonce(\"fusewp_{id}_auth\");\n        binds the round trip to the originating WordPress admin session.\n    - name: redirect_url\n      in: query\n      required: true\n      description: URL-encoded return address on the customer's own WordPress admin.\n    behaviour: 302 to the partner platform's own authorize endpoint.\n  - flow: refreshToken\n    initiation: GET https://auth.fusewp.com/{integration_id}?refresh_token={token}\n    response: JSON object carrying a boolean `success` field plus refreshed credentials\n\
  \    error_handling: >-\n      The plugin treats any response without `success: true` as a failure and\n      increments a local refresh-error counter that feeds a client-side rate\n      limiter (see rate-limits/fusewp-rate-limits.yml).\n    transport_note: >-\n      Called with wp_remote_get and sslverify enabled outside the vendor's local\n      development constant.\n  integration_ids_live:\n  - {id: aweber, partner: AWeber, status: 302}\n  - {id: birdsend, partner: BirdSend, status: 302}\n  - {id: campaignmonitor, partner: Campaign Monitor, status: 302}\n  - {id: constantcontact, partner: Constant Contact, status: 302}\n  - {id: copper, partner: Copper CRM, status: 302}\n  - {id: gohl, partner: GoHighLevel, status: 302}\n  - {id: hubspot, partner: HubSpot, status: 302}\n  - {id: keap, partner: Keap / Infusionsoft, status: 302}\n  - {id: mailchimp, partner: Mailchimp, status: 302}\n  - {id: zohocampaigns, partner: Zoho Campaigns, status: 302}\n  - {id: zohocrm, partner: Zoho CRM, status:\
  \ 302}\n  integration_ids_erroring:\n  - {id: google_sheet, partner: Google Sheets, status: 500}\n  - {id: salesforce, partner: Salesforce, status: 500}\n  erroring_note: >-\n    Both are documented Pro integrations whose broker path returned HTTP 500 on\n    2026-08-12 with an empty body. Recorded as observed; the cause was not\n    determined and this is not asserted to be a permanent outage.\n- id: mcp-oauth\n  name: fusewp.com MCP OAuth server\n  host: https://fusewp.com\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://fusewp.com/oauth/authorize\n    tokenUrl: https://fusewp.com/oauth/token\n    revocationUrl: https://fusewp.com/oauth/revoke\n    pkce: S256\n    scopes: [mcp]\n  client_auth: none (public client, client_id metadata document supported)\n  bearer_methods: [header]\n  protects: https://fusewp.com/wp-json/mcp/mcp-oauth-server\n  source: well-known/fusewp-oauth-authorization-server.json\n  note: >-\n    Emitted by the WordPress MCP Adapter\
  \ on FuseWP's own site. See\n    mcp/fusewp-mcp.yml.\n- id: partner-api-keys\n  name: Partner API key entry\n  type: apiKey\n  in: admin-form\n  role: >-\n    For the ~25 partner platforms that do not use OAuth (ActiveCampaign,\n    Klaviyo, Brevo, MailerLite, ConvertKit/Kit, Drip, GetResponse,\n    EmailOctopus, Encharge, Engage.so, Flodesk, Mailjet, Mailercloud,\n    Omnisend, Ortto, Sender, SendPulse, Sendy, beehiiv, Bento, FluentCRM,\n    Groundhogg, MailPoet and others) the site administrator pastes the\n    partner's own API key or key+URL pair into the FuseWP settings screen. The\n    credential is stored in the customer's WordPress options table and used\n    directly against the partner API — it never traverses a FuseWP-operated\n    service.\n  storage: WordPress options table on the customer's own installation\n- id: license-activation\n  name: License activation\n  host: https://fusewp.com\n  type: apiKey\n  role: >-\n    The Pro build activates against Easy Digital Downloads\
  \ Software Licensing\n    on fusewp.com. The `edd-sl` and `edd` REST namespaces are registered on\n    fusewp.com/wp-json/ and were observed in the namespace listing; the license\n    key is issued to the customer at https://fusewp.com/account/.\n  evidence: namespaces edd, edd-sl, edd/webhooks/v1 present at https://fusewp.com/wp-json/\ninbound_api_of_own:\n  present: false\n  note: >-\n    Grepped the entire shipped plugin for register_rest_route and WP_REST\n    handlers — there are zero. FuseWP exposes no REST API on the customer's\n    WordPress site. Its extension surface is PHP actions and filters\n    (fusewp_loaded, fusewp_profile_update, fusewp_queued_job_handler,\n    fusewp_disable_rate_limiting, fusewp_after_save_oauth_credentials and\n    similar), which are in-process and not addressable over HTTP.\nx-evidence:\n  fetched: '2026-08-12'\n  probes:\n  - {url: 'https://auth.fusewp.com/mailchimp', status: 302}\n  - {url: 'https://auth.fusewp.com/hubspot', status: 302}\n  - {url:\
  \ 'https://auth.fusewp.com/salesforce', status: 500}\n  - {url: 'https://fusewp.com/.well-known/oauth-authorization-server/', status: 200}\n  source_artifact: downloads.wordpress.org/plugin/fusewp.1.1.26.1.zip\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fusewp/refs/heads/main/authentication/fusewp-authentication.yml
summary_line: oauth2/apiKey · 0 schemes
tags:
- Company
- WordPress
- Email Marketing
- Marketing Automation
- CRM
- Integration
- Data Synchronization
- OAuth
- Plugins
- No Code
---
