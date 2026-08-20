---
api_key_in: []
api_specs:
- filename: spredfast-conversations-api-openapi.yml
  format: yaml
  label: Spredfast Conversations API (v2)
  slug: spredfast-conversations-api-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spredfast/refs/heads/main/openapi/spredfast-conversations-api-openapi.yml
- filename: spredfast-conversations-api-v1-openapi.yml
  format: yaml
  label: Spredfast Conversations API (v1)
  slug: spredfast-conversations-api-v1
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spredfast/refs/heads/main/openapi/spredfast-conversations-api-v1-openapi.yml
- filename: spredfast-analytics-api-openapi.yml
  format: yaml
  label: Spredfast Analytics Reporting API
  slug: spredfast-analytics-reporting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spredfast/refs/heads/main/openapi/spredfast-analytics-api-openapi.yml
- filename: spredfast-notification-api-openapi.yml
  format: yaml
  label: Spredfast Notifications (Events) API
  slug: spredfast-notifications-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spredfast/refs/heads/main/openapi/spredfast-notification-api-openapi.yml
- filename: spredfast-experiences-stream-api-openapi.yml
  format: yaml
  label: Spredfast Experiences Stream API
  slug: spredfast-experiences-stream-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spredfast/refs/heads/main/openapi/spredfast-experiences-stream-api-openapi.yml
- filename: spredfast-crm-api-openapi.yml
  format: yaml
  label: Spredfast CRM Registration API
  slug: spredfast-crm-registration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spredfast/refs/heads/main/openapi/spredfast-crm-api-openapi.yml
- filename: spredfast-custom-crm-callback-api-openapi.yml
  format: yaml
  label: Spredfast Custom CRM Callback Contract
  slug: spredfast-custom-crm-callback-contract
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spredfast/refs/heads/main/openapi/spredfast-custom-crm-callback-api-openapi.yml
- filename: spredfast-labelsets-api-openapi.yml
  format: yaml
  label: Spredfast Label Sets API
  slug: spredfast-label-sets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spredfast/refs/heads/main/openapi/spredfast-labelsets-api-openapi.yml
- filename: spredfast-introspection-api-openapi.yml
  format: yaml
  label: Spredfast Introspection API
  slug: spredfast-introspection-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spredfast/refs/heads/main/openapi/spredfast-introspection-api-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Spredfast Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Spredfast secures its APIs with oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Spredfast
provider_slug: spredfast
scheme_count: 2
schemes:
- authoritative: true
  flows:
  - authorizationUrl: https://login.spredfast.com/v3/oauth/authorize
    description: 3-legged OAuth 2.0 browser redirection flow. Redirect the user to the authorization URL with client_id, response_type=code, redirect_uri and state; exchange the returned code at the token URL with client_id, client_secret and redirect_uri. The response carries a Token object ({ sfEntityType, accessToken, expiryTime }) inside the standard platform envelope.
    flow: authorizationCode
    scopes:
      all: Read/write access for all endpoints.
    tokenUrl: https://login.spredfast.com/v3/oauth/token
  name: oauth2
  sources:
  - openapi/spredfast-conversations-api-v1-openapi.yml
  - https://developer.khoros.com/khorosmarketingdevdocs/docs/getting-started-with-the-conversations-api
  type: oauth2
- authoritative: false
  defect: placeholder-token-url
  flows:
  - description: As published by the provider. The tokenUrl is example.com — an IANA reserved domain — so this flow is not callable as declared. It appears identically in eight of the nine contracts, which is the signature of a docs-platform default rather than a design decision.
    flow: clientCredentials
    scopes: {}
    tokenUrl: https://example.com/oauth2/token
  name: sec0
  sources:
  - openapi/spredfast-conversations-api-openapi.yml
  - openapi/spredfast-analytics-api-openapi.yml
  - openapi/spredfast-crm-api-openapi.yml
  - openapi/spredfast-notification-api-openapi.yml
  - openapi/spredfast-labelsets-api-openapi.yml
  - openapi/spredfast-introspection-api-openapi.yml
  - openapi/spredfast-experiences-stream-api-openapi.yml
  type: oauth2
slug: spredfast-authentication
source_filename: spredfast-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: https://developer.khoros.com/khorosmarketingdevdocs/docs/getting-started-with-the-conversations-api\ndocs: https://developer.khoros.com/khorosmarketingdevdocs\nderived_from:\n- openapi/spredfast-conversations-api-v1-openapi.yml\n- openapi/spredfast-conversations-api-openapi.yml\n- openapi/spredfast-analytics-api-openapi.yml\n- openapi/spredfast-crm-api-openapi.yml\n- openapi/spredfast-notification-api-openapi.yml\n- openapi/spredfast-labelsets-api-openapi.yml\n- openapi/spredfast-introspection-api-openapi.yml\n- openapi/spredfast-experiences-stream-api-openapi.yml\nnote: >-\n  UPGRADED 2026-08-13. The prior round recorded \"No OpenAPI/Swagger definition\n  is published\" — that is now superseded: nine OpenAPI documents were harvested\n  from the Khoros Marketing developer center and are in openapi/. The auth\n  profile is now corroborated by both the docs AND the contracts.\n  IMPORTANT DISCREPANCY: eight of the nine documents\
  \ declare a securityScheme\n  named `sec0` with a `clientCredentials` flow whose tokenUrl is\n  `https://example.com/oauth2/token`. That is a DOCUMENTATION-TOOL PLACEHOLDER\n  (ReadMe's default when a spec is authored in its API Designer), not a\n  Spredfast endpoint — example.com is the IANA reserved domain. The\n  authoritative scheme is the one on the Conversations V1 contract, which names\n  the real Spredfast OAuth host, and it matches the getting-started guide's\n  description of \"3-legged OAuth 2.0\". Treat the placeholder as a defect in the\n  provider's published contracts, not as a second supported flow.\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\n  api_key: false\n  basic_auth: false\n  mtls: false\n  openid_connect: false\n  discovery_metadata: false\naccess_model:\n  self_serve: false\n  note: >-\n    Credentials are issued by Khoros support, not by a developer portal. The\n    company admin must ask support to (a) enable the DevCenter application\
  \ for\n    the company and (b) issue a client id and client secret. That client id must\n    then be allow-listed for the company in Conversations. Until both are done,\n    every call fails with \"Company {id} does not allow the application\n    {clientId}\".\nschemes:\n- name: oauth2\n  type: oauth2\n  authoritative: true\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://login.spredfast.com/v3/oauth/authorize\n    tokenUrl: https://login.spredfast.com/v3/oauth/token\n    scopes:\n      all: Read/write access for all endpoints.\n    description: >-\n      3-legged OAuth 2.0 browser redirection flow. Redirect the user to the\n      authorization URL with client_id, response_type=code, redirect_uri and\n      state; exchange the returned code at the token URL with client_id,\n      client_secret and redirect_uri. The response carries a Token object\n      ({ sfEntityType, accessToken, expiryTime }) inside the standard platform\n      envelope.\n  sources:\n  - openapi/spredfast-conversations-api-v1-openapi.yml\n\
  \  - https://developer.khoros.com/khorosmarketingdevdocs/docs/getting-started-with-the-conversations-api\n- name: sec0\n  type: oauth2\n  authoritative: false\n  defect: placeholder-token-url\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://example.com/oauth2/token\n    scopes: {}\n    description: >-\n      As published by the provider. The tokenUrl is example.com — an IANA\n      reserved domain — so this flow is not callable as declared. It appears\n      identically in eight of the nine contracts, which is the signature of a\n      docs-platform default rather than a design decision.\n  sources:\n  - openapi/spredfast-conversations-api-openapi.yml\n  - openapi/spredfast-analytics-api-openapi.yml\n  - openapi/spredfast-crm-api-openapi.yml\n  - openapi/spredfast-notification-api-openapi.yml\n  - openapi/spredfast-labelsets-api-openapi.yml\n  - openapi/spredfast-introspection-api-openapi.yml\n  - openapi/spredfast-experiences-stream-api-openapi.yml\ntoken:\n  type: bearer\n\
  \  presentation: Authorization header on every API call.\n  lifetime: 24 months (2 years)\n  persists_across_password_change: true\n  refresh: Repeat the authorization flow; there is no separate refresh_token grant documented.\n  revocation: By the authenticating user, in Profile Settings -> Notifications.\n  self_service_issue: >-\n    A user may also generate an API Access Token directly from the Profile\n    Settings area of Khoros Marketing.\n  introspection:\n    supported: true\n    operation: GET https://api.spredfast.com/v2/whoami\n    spec: openapi/spredfast-introspection-api-openapi.yml\n  expiry_signal: >-\n    An expired or revoked token does NOT return a JSON 401 — the docs record an\n    HTML page reading \"Developer Inactive\". Detect it as a content-type\n    mismatch, not a status code.\nenterprise_sso:\n  supported: true\n  note: >-\n    All company security policies, including SAML SSO integration, are enforced\n    during the OAuth login, because OAuth tokens are managed\
  \ by the same\n    authentication system as web logins.\n  source: openapi/spredfast-conversations-api-v1-openapi.yml\nscopes:\n  count: 1\n  note: >-\n    A single scope, `all`, granting read/write across every endpoint. There is\n    no read-only credential, so a reporting integration must be issued the same\n    privilege as a publishing one.\n  detail: scopes/spredfast-scopes.yml\ngaps:\n- No /.well-known/oauth-authorization-server (RFC 8414) — login.spredfast.com returns 404.\n- No /.well-known/openid-configuration — login.spredfast.com returns 404.\n- No PKCE guidance published for the authorization code flow.\n- Client credentials are issued by a support ticket, so there is no programmatic credential lifecycle.\n- >-\n  Eight of nine published contracts declare an uncallable placeholder tokenUrl\n  (example.com), which will mislead any tool that generates a client from them.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/spredfast/refs/heads/main/authentication/spredfast-authentication.yml
summary_line: oauth2 · 2 schemes
tags:
- Company
- Social-Media
- Social Media Management
- Marketing
- Social Marketing
- Publishing
- Analytics
- Engagement
- Content Management
- Webhook
- Event
- Enterprise
---
