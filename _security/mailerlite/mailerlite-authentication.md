---
api_key_in:
- header
api_specs:
- filename: mailerlite-automations-api-openapi.yml
  format: yaml
  label: MailerLite Automations API
  slug: mailerlite-automations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mailerlite/refs/heads/main/openapi/mailerlite-automations-api-openapi.yml
- filename: mailerlite-campaigns-api-openapi.yml
  format: yaml
  label: MailerLite Campaigns API
  slug: mailerlite-campaigns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mailerlite/refs/heads/main/openapi/mailerlite-campaigns-api-openapi.yml
- filename: mailerlite-fields-api-openapi.yml
  format: yaml
  label: MailerLite Fields API
  slug: mailerlite-fields-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mailerlite/refs/heads/main/openapi/mailerlite-fields-api-openapi.yml
- filename: mailerlite-forms-api-openapi.yml
  format: yaml
  label: MailerLite Forms API
  slug: mailerlite-forms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mailerlite/refs/heads/main/openapi/mailerlite-forms-api-openapi.yml
- filename: mailerlite-groups-api-openapi.yml
  format: yaml
  label: MailerLite Groups API
  slug: mailerlite-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mailerlite/refs/heads/main/openapi/mailerlite-groups-api-openapi.yml
- filename: mailerlite-segments-api-openapi.yml
  format: yaml
  label: MailerLite Segments API
  slug: mailerlite-segments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mailerlite/refs/heads/main/openapi/mailerlite-segments-api-openapi.yml
- filename: mailerlite-subscribers-api-openapi.yml
  format: yaml
  label: MailerLite Subscribers API
  slug: mailerlite-subscribers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mailerlite/refs/heads/main/openapi/mailerlite-subscribers-api-openapi.yml
- filename: mailerlite-webhooks-api-openapi.yml
  format: yaml
  label: MailerLite Webhooks API
  slug: mailerlite-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mailerlite/refs/heads/main/openapi/mailerlite-webhooks-api-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Mailerlite Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: MailerLite secures its APIs with http and oauth2 across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: MailerLite
provider_slug: mailerlite
scheme_count: 3
schemes:
- description: API key generated in the MailerLite dashboard under Integrations > MailerLite API > "Generate new token".
  docs: https://developers.mailerlite.com/getting-started
  failure: '401 {"message": "Unauthenticated."}'
  format: Bearer <api key>
  header: Authorization
  in: header
  key_properties:
    bound_to_user: true
    expiring: false
    named: true
    rotatable: true
    scoped: false
    shown_once: true
    stored_plaintext_by_provider: false
  lifecycle_warning: Keys are permanently bound to the user who created them. Removing that user from the account — or deleting their user account — silently kills every integration using that key. There is no service-account concept.
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/mailerlite-subscribers-api-openapi.yml
  - openapi/mailerlite-groups-api-openapi.yml
  - openapi/mailerlite-segments-api-openapi.yml
  - openapi/mailerlite-fields-api-openapi.yml
  - openapi/mailerlite-campaigns-api-openapi.yml
  - openapi/mailerlite-automations-api-openapi.yml
  - openapi/mailerlite-forms-api-openapi.yml
  - openapi/mailerlite-webhooks-api-openapi.yml
  surface: rest
  type: http
- bearer_methods_supported:
  - header
  code_challenge_methods:
  - plain
  - S256
  description: OAuth 2.1-shaped authorization for the hosted MCP server, discovered through RFC 8414 + RFC 9728 metadata. No scopes are advertised — an issued token carries whatever the authorizing MailerLite user can do.
  dynamic_client_registration: true
  flows:
  - authorizationUrl: https://mcp.mailerlite.com/authorize
    flow: authorizationCode
    refreshUrl: https://mcp.mailerlite.com/token
    scopes: {}
    tokenUrl: https://mcp.mailerlite.com/token
  metadata:
    authorization_server: https://mcp.mailerlite.com/.well-known/oauth-authorization-server
    protected_resource: https://mcp.mailerlite.com/.well-known/oauth-protected-resource/mcp
  name: OAuth2 (MCP)
  probe:
    date: '2026-08-13'
    http_status: 401
    method: POST
    url: https://mcp.mailerlite.com/mcp
    www_authenticate: Bearer realm="OAuth", resource_metadata="https://mcp.mailerlite.com/.well-known/oauth-protected-resource/mcp", error="invalid_token"
  registration_endpoint: https://mcp.mailerlite.com/register
  resource: https://mcp.mailerlite.com/mcp
  revocation_endpoint: https://mcp.mailerlite.com/token
  sources:
  - https://mcp.mailerlite.com/.well-known/oauth-authorization-server
  - https://developers.mailerlite.com/mcp
  surface: mcp
  token_endpoint_auth_methods:
  - client_secret_basic
  - client_secret_post
  - none
  type: oauth2
- description: '`mailerlite auth login` is browser-based OAuth and is the CLI''s recommended default; tokens auto-refresh. `--method token` falls back to pasting a dashboard API key, and MAILERLITE_API_TOKEN covers CI.'
  docs: https://developers.mailerlite.com/cli
  flows:
  - flow: authorizationCode
  name: OAuth2 (CLI)
  sources:
  - https://developers.mailerlite.com/cli
  surface: cli
  type: oauth2
slug: mailerlite-authentication
source_filename: mailerlite-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: openapi/*.yml (securitySchemes)\ndocs: https://developers.mailerlite.com/getting-started\nalso:\n  - https://developers.mailerlite.com/cli\n  - https://developers.mailerlite.com/mcp\n  - https://mcp.mailerlite.com/.well-known/oauth-authorization-server\nnotes: >-\n  Upgraded from derived to searched on 2026-08-13. The OpenAPI-only view showed\n  a single bearer scheme; the docs show a THREE-SURFACE auth model in which the\n  REST API is API-key-only while the CLI and the hosted MCP server both use\n  OAuth. That distinction matters to an agent: the callable-by-agent surface\n  (MCP) is OAuth with open Dynamic Client Registration, so an agent can\n  authorize itself, while the REST surface requires a human to mint a key in\n  the dashboard first.\n\nsummary:\n  types: [http, oauth2]\n  api_key_in: [header]\n  oauth2_flows: [authorizationCode]\n  oauth2_scopes: 0\n  surfaces: [rest, cli, mcp]\n  human_bootstrap_required_for_rest:\
  \ true\n\nschemes:\n  - name: BearerAuth\n    type: http\n    scheme: bearer\n    surface: rest\n    in: header\n    header: Authorization\n    format: \"Bearer <api key>\"\n    description: >-\n      API key generated in the MailerLite dashboard under\n      Integrations > MailerLite API > \"Generate new token\".\n    docs: https://developers.mailerlite.com/getting-started\n    sources:\n      - openapi/mailerlite-subscribers-api-openapi.yml\n      - openapi/mailerlite-groups-api-openapi.yml\n      - openapi/mailerlite-segments-api-openapi.yml\n      - openapi/mailerlite-fields-api-openapi.yml\n      - openapi/mailerlite-campaigns-api-openapi.yml\n      - openapi/mailerlite-automations-api-openapi.yml\n      - openapi/mailerlite-forms-api-openapi.yml\n      - openapi/mailerlite-webhooks-api-openapi.yml\n    key_properties:\n      shown_once: true\n      stored_plaintext_by_provider: false\n      rotatable: true\n      scoped: false\n      expiring: false\n      named: true\n      bound_to_user:\
  \ true\n    lifecycle_warning: >-\n      Keys are permanently bound to the user who created them. Removing that\n      user from the account — or deleting their user account — silently kills\n      every integration using that key. There is no service-account concept.\n    failure: '401 {\"message\": \"Unauthenticated.\"}'\n\n  - name: OAuth2 (MCP)\n    type: oauth2\n    surface: mcp\n    resource: https://mcp.mailerlite.com/mcp\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://mcp.mailerlite.com/authorize\n        tokenUrl: https://mcp.mailerlite.com/token\n        refreshUrl: https://mcp.mailerlite.com/token\n        scopes: {}\n    registration_endpoint: https://mcp.mailerlite.com/register\n    revocation_endpoint: https://mcp.mailerlite.com/token\n    code_challenge_methods: [plain, S256]\n    token_endpoint_auth_methods: [client_secret_basic, client_secret_post, none]\n    dynamic_client_registration: true\n    bearer_methods_supported: [header]\n   \
  \ metadata:\n      authorization_server: https://mcp.mailerlite.com/.well-known/oauth-authorization-server\n      protected_resource: https://mcp.mailerlite.com/.well-known/oauth-protected-resource/mcp\n    description: >-\n      OAuth 2.1-shaped authorization for the hosted MCP server, discovered\n      through RFC 8414 + RFC 9728 metadata. No scopes are advertised — an\n      issued token carries whatever the authorizing MailerLite user can do.\n    probe:\n      url: https://mcp.mailerlite.com/mcp\n      method: POST\n      date: '2026-08-13'\n      http_status: 401\n      www_authenticate: >-\n        Bearer realm=\"OAuth\",\n        resource_metadata=\"https://mcp.mailerlite.com/.well-known/oauth-protected-resource/mcp\",\n        error=\"invalid_token\"\n    sources:\n      - https://mcp.mailerlite.com/.well-known/oauth-authorization-server\n      - https://developers.mailerlite.com/mcp\n\n  - name: OAuth2 (CLI)\n    type: oauth2\n    surface: cli\n    flows:\n      - flow: authorizationCode\n\
  \    description: >-\n      `mailerlite auth login` is browser-based OAuth and is the CLI's\n      recommended default; tokens auto-refresh. `--method token` falls back to\n      pasting a dashboard API key, and MAILERLITE_API_TOKEN covers CI.\n    docs: https://developers.mailerlite.com/cli\n    sources:\n      - https://developers.mailerlite.com/cli\n\nwebhook_authentication:\n  direction: inbound-to-customer\n  mechanism: HMAC-SHA256\n  header: Signature\n  key: The webhook `secret` returned when the webhook is created\n  signed_material: raw JSON request body\n  timestamp_in_signature: false\n  replay_protection: >-\n    None published — no timestamp is signed and no tolerance window is\n    documented. Receivers must add their own replay defence.\n  docs: https://developers.mailerlite.com/api/webhooks\n\nnot_supported:\n  - openIdConnect\n  - mutualTLS\n  - basic auth\n  - hmac request signing on outbound REST calls\n  - scoped / least-privilege API keys\n  - key expiry\n\ngaps:\n\
  \  - >-\n    No scope surface anywhere: neither the REST keys nor the MCP OAuth tokens\n    can be narrowed. A token that can list subscribers can also schedule a\n    campaign send.\n  - >-\n    No service-account identity — API keys inherit and die with a human user.\n\nmaintainers:\n  - FN: Kin Lane\n    email: kin@apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mailerlite/refs/heads/main/authentication/mailerlite-authentication.yml
summary_line: http/oauth2 · 3 schemes
tags:
- Email Marketing
- Automation
- Newsletters
- Subscribers
- Campaigns
- Webhook
- E-Commerce
- Segmentation
- Transactional Email
- MCP
---
