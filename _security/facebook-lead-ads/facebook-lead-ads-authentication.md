---
api_key_in: []
api_specs:
- filename: facebook-lead-ads-bulk-leads-api-openapi.yml
  format: yaml
  label: Facebook Lead Ads Bulk Leads API
  slug: facebook-lead-ads-bulk-leads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/facebook-lead-ads/refs/heads/main/openapi/facebook-lead-ads-bulk-leads-api-openapi.yml
- filename: facebook-lead-ads-leadgen-forms-api-openapi.yml
  format: yaml
  label: Facebook Lead Ads Leadgen Forms API
  slug: facebook-lead-ads-leadgen-forms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/facebook-lead-ads/refs/heads/main/openapi/facebook-lead-ads-leadgen-forms-api-openapi.yml
- filename: facebook-lead-ads-leads-api-openapi.yml
  format: yaml
  label: Facebook Lead Ads Leads API
  slug: facebook-lead-ads-leads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/facebook-lead-ads/refs/heads/main/openapi/facebook-lead-ads-leads-api-openapi.yml
- filename: facebook-lead-ads-meta-marketing-api-lead-ads-api-openapi.yml
  format: yaml
  label: Facebook Lead Ads Meta Marketing API Lead Ads API
  slug: facebook-lead-ads-meta-marketing-api-lead-ads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/facebook-lead-ads/refs/heads/main/openapi/facebook-lead-ads-meta-marketing-api-lead-ads-api-openapi.yml
- filename: facebook-lead-ads-subscribed-apps-api-openapi.yml
  format: yaml
  label: Facebook Lead Ads Subscribed Apps API
  slug: facebook-lead-ads-subscribed-apps-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/facebook-lead-ads/refs/heads/main/openapi/facebook-lead-ads-subscribed-apps-api-openapi.yml
- filename: facebook-lead-ads-subscriptions-api-openapi.yml
  format: yaml
  label: Facebook Lead Ads Subscriptions API
  slug: facebook-lead-ads-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/facebook-lead-ads/refs/heads/main/openapi/facebook-lead-ads-subscriptions-api-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Facebook Lead Ads Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Facebook Lead Ads secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Facebook Lead Ads
provider_slug: facebook-lead-ads
scheme_count: 1
schemes:
- description: 'Page access token obtained via Facebook Login / Meta Business

    Login with leads_retrieval, pages_show_list, and

    pages_manage_ads permissions.'
  flows:
  - authorizationUrl: https://www.facebook.com/v22.0/dialog/oauth
    flow: authorizationCode
    scopes: 6
    tokenUrl: https://graph.facebook.com/v22.0/oauth/access_token
  name: PageAccessToken
  sources:
  - openapi/facebook-lead-ads-openapi.yml
  type: oauth2
slug: facebook-lead-ads-authentication
source_filename: facebook-lead-ads-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-14'\nmethod: searched\nsource: openapi/facebook-lead-ads-openapi.yml\ndocs: https://developers.facebook.com/docs/facebook-login/guides/access-tokens\nalso:\n  - https://www.facebook.com/.well-known/openid-configuration\n  - https://developers.facebook.com/docs/marketing-api/guides/lead-ads/retrieving\nnote: >-\n  Upgraded from derived to searched. The OpenAPI declares a single oauth2 scheme; this file\n  adds the token TYPES Meta actually issues (the spec models only one of them), the live\n  auth challenge observed on the wire, and the OIDC discovery document that sits behind the\n  same login.\nsummary:\n  types: [oauth2]\n  oauth2_flows: [authorizationCode]\n  oidc_discovery: true\n  api_key: false\n  mutual_tls: false\nschemes:\n  - name: PageAccessToken\n    type: oauth2\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://www.facebook.com/v22.0/dialog/oauth\n        tokenUrl: https://graph.facebook.com/v22.0/oauth/access_token\n\
  \        scopes: 6\n    description: |-\n      Page access token obtained via Facebook Login / Meta Business\n      Login with leads_retrieval, pages_show_list, and\n      pages_manage_ads permissions.\n    sources:\n      - openapi/facebook-lead-ads-openapi.yml\ntransport:\n  - 'Authorization: Bearer <access_token>'\n  - '?access_token=<access_token> query parameter (also accepted)'\nobserved_challenge:\n  fetched: '2026-08-14'\n  url: https://graph.facebook.com/v22.0/me\n  http_status: 400\n  header: >-\n    www-authenticate: OAuth \"Facebook Platform\" \"invalid_request\" \"An active access token\n    must be used to query information about the current user.\"\ntoken_types:\n  - name: Page access token\n    modeled_in_spec: true\n    description: >-\n      The token this API requires. Issued to an app for a specific Page by a Page admin.\n      Every lead-ads read is scoped to the Page that owns the form.\n  - name: User access token\n    modeled_in_spec: false\n    description: >-\n\
  \      Issued by Facebook Login to act on behalf of a person. Used to enumerate the Pages a\n      user administers (pages_show_list) before exchanging for a Page token.\n  - name: System user access token\n    modeled_in_spec: false\n    description: >-\n      Long-lived, non-human credential created in Meta Business Suite. The credential\n      Meta's own Ads CLI authenticates with, and the right choice for unattended\n      server-to-server lead sync.\n    reference: cli/facebook-lead-ads-cli.yml\n  - name: App access token\n    modeled_in_spec: false\n    description: >-\n      app-id|app-secret. Used for app-level configuration such as the webhook subscription\n      on /{app-id}/subscriptions.\noidc:\n  discovery: https://www.facebook.com/.well-known/openid-configuration\n  probed: '2026-08-14'\n  http_status: 200\n  issuer: https://www.facebook.com\n  authorization_endpoint: https://facebook.com/dialog/oauth/\n  jwks_uri: https://www.facebook.com/.well-known/oauth/openid/jwks/\n\
  \  response_types_supported: [id_token, 'token id_token']\n  subject_types_supported: [pairwise]\n  id_token_signing_alg_values_supported: [RS256]\n  file: well-known/facebook-lead-ads-openid-configuration.json\n  note: >-\n    This is the Facebook Login OIDC surface behind the same authorization dialog. It offers\n    only implicit-style response types — \"code\" is not in response_types_supported — so the\n    authorizationCode flow the API uses is Meta's own OAuth 2.0 implementation, not the OIDC\n    code flow.\ndiscovery_gaps:\n  rfc8414_authorization_server_metadata: false\n  rfc9728_protected_resource_metadata: false\n  note: >-\n    Neither /.well-known/oauth-authorization-server nor\n    /.well-known/oauth-protected-resource is served on any host, so an OAuth client cannot\n    machine-discover the endpoints — they must be hard-coded from the docs. See\n    well-known/facebook-lead-ads-well-known.yml.\nwebhook_authentication:\n  outbound: X-Hub-Signature-256 (HMAC-SHA256 over\
  \ the raw body, keyed by the app secret)\n  handshake: hub.verify_token compared against the App Dashboard value\n  detail: asyncapi/facebook-lead-ads-webhooks.yml\nscopes_detail: scopes/facebook-lead-ads-scopes.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/facebook-lead-ads/refs/heads/main/authentication/facebook-lead-ads-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Advertising
- Lead Generation
- Lead Ads
- Marketing API
- Facebook
- Instagram
- Meta
- Webhook
---
