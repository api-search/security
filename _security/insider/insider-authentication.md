---
api_key_in:
- header
api_specs:
- filename: insider-unification-openapi.yml
  format: yaml
  label: Insider One Unification API
  slug: insider-one-unification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/insider/refs/heads/main/openapi/insider-unification-openapi.yml
- filename: insider-contact-openapi.yml
  format: yaml
  label: Insider One Contact API
  slug: insider-one-contact-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/insider/refs/heads/main/openapi/insider-contact-openapi.yml
- filename: insider-mail-openapi.yml
  format: yaml
  label: Insider One Mail API
  slug: insider-one-mail-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/insider/refs/heads/main/openapi/insider-mail-openapi.yml
- filename: insider-sms-openapi.yml
  format: yaml
  label: Insider One SMS API
  slug: insider-one-sms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/insider/refs/heads/main/openapi/insider-sms-openapi.yml
- filename: insider-whatsapp-openapi.yml
  format: yaml
  label: Insider One WhatsApp API
  slug: insider-one-whatsapp-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/insider/refs/heads/main/openapi/insider-whatsapp-openapi.yml
- filename: insider-gateway-openapi.yml
  format: yaml
  label: Insider One Gateway API (OAuth 2.0)
  slug: insider-one-gateway-api-oauth-20
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/insider/refs/heads/main/openapi/insider-gateway-openapi.yml
- filename: insider-web-push-openapi.yml
  format: yaml
  label: Insider One Web Push API
  slug: insider-one-web-push-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/insider/refs/heads/main/openapi/insider-web-push-openapi.yml
- filename: insider-mobile-openapi.yml
  format: yaml
  label: Insider One Mobile App API
  slug: insider-one-mobile-app-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/insider/refs/heads/main/openapi/insider-mobile-openapi.yml
- filename: insider-mobile-settings-openapi.yml
  format: yaml
  label: Insider One Mobile Settings API
  slug: insider-one-mobile-settings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/insider/refs/heads/main/openapi/insider-mobile-settings-openapi.yml
- filename: insider-live-activity-openapi.yml
  format: yaml
  label: Insider One Live Activity API
  slug: insider-one-live-activity-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/insider/refs/heads/main/openapi/insider-live-activity-openapi.yml
- filename: insider-verify-openapi.yml
  format: yaml
  label: Insider One Verify (OTP) API
  slug: insider-one-verify-otp-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/insider/refs/heads/main/openapi/insider-verify-openapi.yml
- filename: insider-catalog-openapi.yml
  format: yaml
  label: Insider One Catalog API
  slug: insider-one-catalog-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/insider/refs/heads/main/openapi/insider-catalog-openapi.yml
- filename: insider-recommendation-openapi.yml
  format: yaml
  label: Insider One Recommendation API
  slug: insider-one-recommendation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/insider/refs/heads/main/openapi/insider-recommendation-openapi.yml
- filename: insider-eureka-search-openapi.yml
  format: yaml
  label: Insider One Eureka Search API
  slug: insider-one-eureka-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/insider/refs/heads/main/openapi/insider-eureka-search-openapi.yml
- filename: insider-eureka-events-openapi.yml
  format: yaml
  label: Insider One Eureka Event Collection API
  slug: insider-one-eureka-event-collection-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/insider/refs/heads/main/openapi/insider-eureka-events-openapi.yml
- filename: insider-analytics-openapi.yml
  format: yaml
  label: Insider One Analytics API
  slug: insider-one-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/insider/refs/heads/main/openapi/insider-analytics-openapi.yml
- filename: insider-architect-analytics-openapi.yml
  format: yaml
  label: Insider One Architect Analytics API
  slug: insider-one-architect-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/insider/refs/heads/main/openapi/insider-architect-analytics-openapi.yml
- filename: insider-architect-transactional-openapi.yml
  format: yaml
  label: Insider One Architect Transactional Journey API
  slug: insider-one-architect-transactional-journey-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/insider/refs/heads/main/openapi/insider-architect-transactional-openapi.yml
auth_types:
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Insider Authentication
name_suffix: Authentication
oauth_flows:
- authorization_code
- client_credentials
- refresh_token
overview: Insider secures its APIs with apiKey and oauth2 across 7 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorization_code, client_credentials, and refresh_token flow(s).
provider_name: Insider
provider_slug: insider
scheme_count: 7
schemes:
- description: The Insider One partner (account) name, lowercase and without spaces. Found in InOne > Inone Settings > Account Settings. Paired with X-REQUEST-TOKEN.
  in: header
  name: PartnerName
  parameter: X-PARTNER-NAME
  sources:
  - docs
  - postman
  type: apiKey
  used_by:
  - unification.useinsider.com
  - contact.useinsider.com
  - mobile.useinsider.com
- description: The account API key (request token) generated in InOne > Settings > Integration Settings.
  in: header
  name: RequestToken
  occurrences_in_collection: 52
  parameter: X-REQUEST-TOKEN
  sources:
  - docs
  - postman
  type: apiKey
  used_by:
  - unification.useinsider.com
  - contact.useinsider.com
  - mobile.useinsider.com
  - analytics.api.useinsider.com
  - architect-analytics.api.useinsider.com
- description: Per-API authorization key used by the messaging and catalog hosts.
  in: header
  name: InsAuthKey
  occurrences_in_collection: 44
  parameter: X-INS-AUTH-KEY
  sources:
  - postman
  type: apiKey
  used_by:
  - sms.useinsider.com
  - whatsapp.useinsider.com
  - verify.useinsider.com
  - mail.useinsider.com
  - catalog.api.useinsider.com
  - web-push.api.useinsider.com
- description: Mobile-suite API key (a second casing, X-API-KEY, also appears in the collection).
  in: header
  name: ApiKey
  parameter: X-Api-Key
  sources:
  - postman
  - docs
  type: apiKey
  used_by:
  - mobile.api.useinsider.com
  - mobile.useinsider.com
- description: Single-use variant seen on one collection request.
  in: header
  name: InsiderApiKey
  parameter: X-INSIDER-API-KEY
  sources:
  - postman
  type: apiKey
- description: Bearer credential. On gw.useinsider.com this carries an OAuth 2.0 access token; on some other hosts the collection uses the same header to carry the channel API key.
  in: header
  name: Authorization
  parameter: Authorization
  scheme: bearer
  sources:
  - postman
  - docs
  type: http
- description: OAuth 2.0 for the Insider One gateway and MCP server. Client ID / Client Secret generated in InOne > Settings > InOne Settings > Integration Settings > OAuth 2.0 Credentials, with the channel scopes selected at generation time.
  discovery: well-known/insider-gw-oauth-authorization-server.json
  flows:
  - authorizationUrl: https://gw.useinsider.com/oauth2/authorize
    flow: authorizationCode
    tokenUrl: https://gw.useinsider.com/oauth2/token
  - flow: clientCredentials
    tokenUrl: https://gw.useinsider.com/oauth2/token
  issuer: https://gw.useinsider.com
  name: OAuth2
  pkce:
  - S256
  refresh: supported (refresh_token grant)
  revocation_endpoint: https://gw.useinsider.com/oauth2/revoke
  sources:
  - well-known
  - docs
  token_endpoint_auth_methods:
  - client_secret_basic
  - client_secret_post
  - none
  token_lifetime: up to 90 minutes
  type: oauth2
  used_by:
  - gw.useinsider.com
  - https://mcp.insiderone.com/mcp
slug: insider-authentication
source_filename: insider-authentication.yml
source_heading: Authentication Profile
source_url: https://academy.insiderone.com/docs/api-authentication-tokens-1
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: https://academy.insiderone.com/docs/api-authentication-tokens-1\ndocs: https://academy.insiderone.com/docs/api-authentication-tokens-1\nsources:\n- https://academy.insiderone.com/docs/api-authentication-tokens-1\n- https://academy.insiderone.com/docs/insider-one-apis-1\n- https://academy.insiderone.com/docs/anatomy-of-an-api-request-1\n- https://academy.insiderone.com/docs/set-up-insider-one-mcp\n- https://gw.useinsider.com/.well-known/oauth-authorization-server\n- postman/insider-one-apis.postman_collection.json\nsummary:\n  types: [apiKey, oauth2]\n  api_key_in: [header]\n  oauth2_flows: [authorization_code, client_credentials, refresh_token]\n  notes: >-\n    Insider One runs TWO authentication regimes side by side. (1) The REST estate is key-based:\n    every request carries an account API key in a header, but the HEADER NAME VARIES BY API — the\n    Unification/UCD APIs take the X-PARTNER-NAME + X-REQUEST-TOKEN pair, while\
  \ other hosts take\n    X-INS-AUTH-KEY, X-Api-Key, X-INSIDER-API-KEY or an Authorization value. There are six distinct\n    key headers in the provider's own Postman collection. Keys are generated per API type in the\n    InOne panel by an Administrator, shown once, and can be pinned to allowed IP addresses.\n    (2) The newer gateway (gw.useinsider.com) and the MCP server use OAuth 2.0, with Client\n    ID/Secret generated in Integration Settings, per-channel scopes chosen at generation time,\n    PKCE S256, and RFC 8414 + RFC 9728 discovery documents served anonymously.\n\nschemes:\n- name: PartnerName\n  type: apiKey\n  in: header\n  parameter: X-PARTNER-NAME\n  description: >-\n    The Insider One partner (account) name, lowercase and without spaces. Found in InOne >\n    Inone Settings > Account Settings. Paired with X-REQUEST-TOKEN.\n  used_by: [unification.useinsider.com, contact.useinsider.com, mobile.useinsider.com]\n  sources: [docs, postman]\n- name: RequestToken\n  type: apiKey\n\
  \  in: header\n  parameter: X-REQUEST-TOKEN\n  description: The account API key (request token) generated in InOne > Settings > Integration Settings.\n  used_by: [unification.useinsider.com, contact.useinsider.com, mobile.useinsider.com, analytics.api.useinsider.com, architect-analytics.api.useinsider.com]\n  occurrences_in_collection: 52\n  sources: [docs, postman]\n- name: InsAuthKey\n  type: apiKey\n  in: header\n  parameter: X-INS-AUTH-KEY\n  description: Per-API authorization key used by the messaging and catalog hosts.\n  used_by: [sms.useinsider.com, whatsapp.useinsider.com, verify.useinsider.com, mail.useinsider.com, catalog.api.useinsider.com, web-push.api.useinsider.com]\n  occurrences_in_collection: 44\n  sources: [postman]\n- name: ApiKey\n  type: apiKey\n  in: header\n  parameter: X-Api-Key\n  description: Mobile-suite API key (a second casing, X-API-KEY, also appears in the collection).\n  used_by: [mobile.api.useinsider.com, mobile.useinsider.com]\n  sources: [postman, docs]\n\
  - name: InsiderApiKey\n  type: apiKey\n  in: header\n  parameter: X-INSIDER-API-KEY\n  description: Single-use variant seen on one collection request.\n  sources: [postman]\n- name: Authorization\n  type: http\n  scheme: bearer\n  in: header\n  parameter: Authorization\n  description: >-\n    Bearer credential. On gw.useinsider.com this carries an OAuth 2.0 access token; on some other\n    hosts the collection uses the same header to carry the channel API key.\n  sources: [postman, docs]\n- name: OAuth2\n  type: oauth2\n  description: >-\n    OAuth 2.0 for the Insider One gateway and MCP server. Client ID / Client Secret generated in\n    InOne > Settings > InOne Settings > Integration Settings > OAuth 2.0 Credentials, with the\n    channel scopes selected at generation time.\n  issuer: https://gw.useinsider.com\n  flows:\n  - {flow: authorizationCode, authorizationUrl: 'https://gw.useinsider.com/oauth2/authorize', tokenUrl: 'https://gw.useinsider.com/oauth2/token'}\n  - {flow: clientCredentials,\
  \ tokenUrl: 'https://gw.useinsider.com/oauth2/token'}\n  refresh: supported (refresh_token grant)\n  revocation_endpoint: https://gw.useinsider.com/oauth2/revoke\n  pkce: [S256]\n  token_endpoint_auth_methods: [client_secret_basic, client_secret_post, none]\n  token_lifetime: up to 90 minutes\n  discovery: well-known/insider-gw-oauth-authorization-server.json\n  used_by: [gw.useinsider.com, 'https://mcp.insiderone.com/mcp']\n  sources: [well-known, docs]\n\nkey_management:\n  who_can_generate: Administrator role only\n  visibility: full key shown once at creation; not retrievable afterwards\n  ip_restriction: supported — allowed IPs are authorized at key generation; transactional keys can also\n    be IP-restricted on request\n  limits:\n  - Two active mobile API keys per account; a third requires deleting one.\n  - Web Push keys created in the legacy Web Push Settings screen were disabled on 2025-10-15.\n  rotation_guidance: >-\n    Documented rotation procedure: generate the replacement\
  \ key with the same authorized IPs, store\n    it in a secrets manager, swap it into every consumer, test, monitor for auth failures, then\n    delete the old key. Keys cannot be rotated automatically.\n  mcp_guidance: Create a dedicated OAuth 2.0 credential for the MCP client; do not reuse existing keys.\n\ngaps:\n- Six different API-key header names across the estate, with two casings of the same header\n  (X-Api-Key / X-API-KEY); a client cannot infer the header from the host.\n- No OpenID Connect discovery (gw.useinsider.com/.well-known/openid-configuration is 404).\n- scopes_supported in the protected-resource metadata is the wildcard \"*\", so the real per-channel\n  scope names are only visible inside the panel — see scopes/insider-scopes.yml.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/insider/refs/heads/main/authentication/insider-authentication.yml
summary_line: apiKey/oauth2 · 7 schemes
tags:
- Company
- Customer Engagement
- Personalization
- Customer Data Platform
- Marketing
- Journey Orchestration
- Omnichannel
- CDP
- Artificial Intelligence
- Messaging
- WhatsApp
- Email
- SMS
- Push Notifications
- Recommendations
- Search
- Product Catalog
- Analytics
- MCP
- Agents
- Consent
- GDPR
---
