---
api_key_in: []
auth_types:
- oauth2
- none
description: Loomly publishes no API authentication documentation. This profile is assembled from what can be probed anonymously and from what Loomly's own help-center articles say about connecting Zapier. Nothing here is taken from a specification, because Loomly publishes none.
kind: authentication
layout: security
method: probed
name: Loomly Authentication
name_suffix: Authentication
oauth_flows:
- authorization_code
overview: Loomly secures its APIs with oauth2 and none across 0 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorization_code flow(s).
provider_name: Loomly
provider_slug: loomly
scheme_count: 0
schemes: []
slug: loomly-authentication
source_filename: loomly-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: >-\n  Live probes of app.loomly.com and status.loomly.com, plus the Loomly Zapier\n  listing and the Loomly help center Zapier articles.\nname: Loomly Authentication\ndescription: >-\n  Loomly publishes no API authentication documentation. This profile is assembled\n  from what can be probed anonymously and from what Loomly's own help-center\n  articles say about connecting Zapier. Nothing here is taken from a\n  specification, because Loomly publishes none.\nsummary:\n  types:\n    - oauth2\n    - none\n  oauth2_flows:\n    - authorization_code\n  documented_by_provider: false\n  spec_derived: false\nsurfaces:\n  - name: Loomly Platform API (partner-gated)\n    auth: oauth2\n    flow: authorization_code\n    authorization_endpoint: https://app.loomly.com/oauth/authorize\n    token_endpoint: null\n    scopes_published: false\n    evidence:\n      - url: https://app.loomly.com/oauth/authorize\n        http_status: 302\n      \
  \  location: https://app.loomly.com/signin?redirect=%2Foauth%2Fauthorize\n        fetched: '2026-08-13'\n        note: >-\n          A distinct, routed OAuth authorization endpoint that redirects\n          unauthenticated callers to sign-in. Sibling paths under /oauth/ (for\n          example /oauth/token) return the application's generic 404 shell, so\n          /oauth/authorize is a real route rather than a catch-all.\n      - url: https://zapier.com/apps/loomly/integrations\n        http_status: 200\n        fetched: '2026-08-13'\n        note: >-\n          The Zapier app is the only publicly named consumer of this API.\n      - url: https://loomly.zendesk.com/hc/en-us/articles/38970621662619-How-to-Use-Zapier-to-Connect-Loomly-with-Other-Apps\n        http_status: 200\n        fetched: '2026-08-13'\n        note: >-\n          Loomly's own help article instructs users to \"Sign in to Loomly\" and\n          \"click on Authorize\" from Zapier — an authorization-code consent flow.\n\
  \    gaps:\n      - No token endpoint is published.\n      - No scope list, consent screen documentation, or token lifetime is published.\n      - No client registration path exists; clients are onboarded by Loomly/Zapier.\n      - No refresh-token, revocation, or rotation policy is published.\n  - name: Loomly Status API\n    auth: none\n    anonymous: true\n    evidence:\n      - url: https://status.loomly.com/api/v1/status\n        http_status: 200\n        content_type: application/json; charset=utf-8\n        fetched: '2026-08-13'\n        note: >-\n          Returns 200 JSON with no Authorization header. Read-only status-page\n          data only. The write side of the same vendor API (api.sorryapp.com)\n          requires a bearer API token, but that token belongs to SorryApp's\n          product, not to a Loomly API program.\ndiscovery:\n  well_known_probed:\n    - url: https://www.loomly.com/.well-known/openid-configuration\n      http_status: 404\n    - url: https://www.loomly.com/.well-known/oauth-authorization-server\n\
  \      http_status: 404\n    - url: https://app.loomly.com/.well-known/openid-configuration\n      http_status: 404\n    - url: https://app.loomly.com/.well-known/oauth-authorization-server\n      http_status: 404\n    - url: https://app.loomly.com/.well-known/oauth-protected-resource\n      http_status: 404\n  note: >-\n    No OAuth 2.0 Authorization Server Metadata (RFC 8414) and no OpenID Connect\n    discovery document is served on any Loomly host, so an agent cannot discover\n    the token endpoint or scopes without a partner conversation.\nnotes:\n  - >-\n    A previous automated pass recorded \"Authenticated via OAuth 2.0 Bearer\n    tokens\" against a base URL of https://api.loomly.com/v1. That host does not\n    exist (NXDOMAIN on 1.1.1.1, 8.8.8.8 and 9.9.9.9 as of 2026-08-13) and no\n    Loomly page names it. That claim has been removed; this file records only\n    what was probed.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/loomly/refs/heads/main/authentication/loomly-authentication.yml
summary_line: oauth2/none · 0 schemes
tags:
- Social-Media
- Content Calendar
- Scheduling
- Approval Workflows
- Analytics
- Brand Management
- Publishing
- Community Management
- Marketing
- Social Media Management
---
