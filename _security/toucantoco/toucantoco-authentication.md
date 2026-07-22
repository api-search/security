---
api_key_in:
- header
auth_types:
- apiKey
- oauth2
- http
description: ''
kind: authentication
layout: security
method: searched
name: Toucantoco Authentication
name_suffix: Authentication
oauth_flows:
- jwt-bearer
overview: Toucan Toco secures its APIs with apiKey, oauth2, and http across 0 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the jwt-bearer flow(s).
provider_name: Toucan Toco
provider_slug: toucantoco
scheme_count: 0
schemes: []
slug: toucantoco-authentication
source_filename: toucantoco-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://docs-v3.toucantoco.com/visualizations-and-layouts/embedding/authentication\ndocs:\n  - https://docs-v3.toucantoco.com/visualizations-and-layouts/embedding/authentication\n  - https://docs-v3.toucantoco.com/visualizations-and-layouts/embedding/embed-sdk/embed-sdk-authentication\n  - https://docs.toucanai.cloud/embed/authentication\n  - https://docs.toucanai.cloud/embed/authentication/how-to/generate-an-api-key\n  - https://docs.toucanai.cloud/embed/authentication/how-to/generate-a-token-via-api\n  - https://docs.toucanai.cloud/embed/authentication/how-to/token-introspection\nsummary:\n  types: [apiKey, oauth2, http]\n  api_key_in: [header]\n  oauth2_flows: [jwt-bearer]\n  notes: Two product generations with distinct auth surfaces (classic Toucan platform and Toucan AI cloud).\nsurfaces:\n  - product: Toucan (classic platform embeds)\n    scheme: oauth2 JWT-bearer assertion exchange\n    detail: >-\n      Embed authentication\
  \ uses the OAuth 2.0 JWT bearer grant\n      (grant_type=urn:ietf:params:oauth:grant-type:jwt-bearer, scope=embed) against a\n      Keycloak-style OpenID Connect token endpoint:\n      POST https://<instance>/api/auth/realms/<tenant>/protocol/openid-connect/token,\n      authenticated with client id toucan-embed-client + client secret. The JWT\n      assertion is signed RS512 with a customer RSA key pair (>=2048 bits, public key\n      uploaded to the admin area) or keys published on a customer-hosted JWKS endpoint\n      (multiple keys, rotation supported). The assertion carries an embed_context\n      (username, workspace_id, roles USER/ADMIN, privileges per app, groups, arbitrary\n      attributes, and non-displayed secrets; max 3.5KB) and is exchanged for an opaque\n      access token passed to the embed script or Embed SDK.\n  - product: Toucan AI (toucanai.cloud)\n    scheme: apiKey -> signed JWT access token\n    detail: >-\n      An organization API key (from User Settings) is\
  \ used server-side via the\n      x-api-key header on POST https://toucanai.cloud/embed/generate-token with a user\n      object (distinctId, role e.g. \"explorer\", attributes for RLS/custom traits). The\n      response returns a signed JWT ({token, expiresIn: \"1h\"}) used as auth-token by\n      the <tc-dashboard>/<tc-ai-assistant> web components and as an Authorization\n      Bearer token on the MCP endpoint (https://toucanai.cloud/api/mcp). A Token\n      Introspection tool in Embed settings decodes user info, custom attributes,\n      permissions (can_view/can_edit/can_query), and expiration. Docs stress\n      server-side-only key handling.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/toucantoco/refs/heads/main/authentication/toucantoco-authentication.yml
summary_line: apiKey/oauth2/http · 0 schemes
tags:
- Analytics
- Business Intelligence
- Embedded Analytics
- Data Visualization
- Data Storytelling
- Dashboards
- AI
---
