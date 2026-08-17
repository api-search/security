---
api_key_in: []
auth_types:
- saml
- openIdConnect
- oauth2
- hmac-signature
description: ''
kind: authentication
layout: security
method: searched
name: Orum Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: Orum secures its APIs with saml, openIdConnect, oauth2, and hmac-signature across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Orum
provider_slug: orum-com
scheme_count: 2
schemes:
- configuration_link_lifetime:
    completion_window: 5 hours after first access
    max_accesses: 10
    valid_for: 5 days from generation
  domain_verification:
    method: DNS record on the authoritative DNS server for the email domain
    required: true
    tip_published: keep the TTL on the verification records short
    typical_duration: 24-48 hours
  enablement: Org admin enables SSO under Settings -> System Settings -> Single Sign-On, then sends a self-service configuration link to an IdP administrator who does not need an Orum account.
  identity_platform: Auth0
  identity_providers_named:
  - Okta
  - Azure AD
  - Google Workspace
  idp_note: Orum names those three and says "and others"; the authoritative list is Auth0's, which Orum defers to rather than publishing its own.
  kind: user-authentication
  mfa:
    note: The security page states "depending on your login method, Orum supports multi-factor authentication" — conditional, with no detail on which methods.
    supported: true
  name: application-sso
  source: https://support.orum.com/en-US/orum/article/Am0DBxe--singlesignon-sso
  sso_only_mode:
    note: 'An org can restrict authentication to SSO only. Orum publishes the failure mode plainly: "In the case where our third party provider, Auth0, is down, access to Orum will not be possible unless this option is disabled." Support must disable it manually to restore access. That is a single-vendor availability dependency on the login path, disclosed.'
    supported: true
  standards:
  - SAML
  - OpenID Connect
  - OAuth 2.0
  type: openIdConnect
- algorithm: HMAC-SHA256
  direction: Orum -> customer endpoint (consumer verifies)
  encoding: base64
  header: x-webhook-signature
  header_format: t={timestamp},s={encoded-signature}
  key_management: 'The signing key is chosen by the customer at webhook-creation time and typed into the Orum UI. Orum does not generate it, does not rotate it, and explicitly permits ignoring it: "you may discard it on receipt if you don''t wish to use a signing key, but something does need to be filled out here." There is no key rotation mechanism and no way to read the key back out.'
  kind: message-authentication
  name: webhook-signature
  replay_protection: Advisory only — Orum recommends rejecting payloads whose timestamp is more than five minutes old. Not enforced by Orum.
  scheme: hmac
  signed_value: '{timestamp}.{stringified_body}'
  source: https://support.orum.com/en-US/orum/article/ART-463-webhooks
  standards_note: not RFC 9421 HTTP Message Signatures and not Standard Webhooks
  type: http
slug: orum-com-authentication
source_filename: orum-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: https://support.orum.com/en-US/orum/article/Am0DBxe--singlesignon-sso\ndocs: https://support.orum.com/en-US/orum/article/Am0DBxe--singlesignon-sso\nscope: >-\n  IMPORTANT — there is no public request API, so there is no API authentication model to\n  document. This file records the two authentication surfaces Orum actually publishes: (1)\n  human sign-in to the Orum application, and (2) the signature scheme a webhook CONSUMER uses\n  to authenticate Orum's outbound deliveries. Nothing here was derived from a spec; there is\n  no spec.\nsummary:\n  types: [saml, openIdConnect, oauth2, hmac-signature]\n  api_key_in: []\n  oauth2_flows: []\n  api_auth_documented: false\n  api_auth_note: no API keys, tokens, or client credentials are issued or documented\n\nschemes:\n- name: application-sso\n  kind: user-authentication\n  type: openIdConnect\n  identity_platform: Auth0\n  standards: [SAML, OpenID Connect, OAuth 2.0]\n  identity_providers_named:\
  \ [Okta, Azure AD, Google Workspace]\n  idp_note: >-\n    Orum names those three and says \"and others\"; the authoritative list is Auth0's, which\n    Orum defers to rather than publishing its own.\n  enablement: >-\n    Org admin enables SSO under Settings -> System Settings -> Single Sign-On, then sends a\n    self-service configuration link to an IdP administrator who does not need an Orum account.\n  configuration_link_lifetime:\n    valid_for: 5 days from generation\n    completion_window: 5 hours after first access\n    max_accesses: 10\n  domain_verification:\n    required: true\n    method: DNS record on the authoritative DNS server for the email domain\n    typical_duration: 24-48 hours\n    tip_published: keep the TTL on the verification records short\n  sso_only_mode:\n    supported: true\n    note: >-\n      An org can restrict authentication to SSO only. Orum publishes the failure mode plainly:\n      \"In the case where our third party provider, Auth0, is down, access to\
  \ Orum will not be\n      possible unless this option is disabled.\" Support must disable it manually to restore\n      access. That is a single-vendor availability dependency on the login path, disclosed.\n  mfa:\n    supported: true\n    note: >-\n      The security page states \"depending on your login method, Orum supports multi-factor\n      authentication\" — conditional, with no detail on which methods.\n  source: https://support.orum.com/en-US/orum/article/Am0DBxe--singlesignon-sso\n\n- name: webhook-signature\n  kind: message-authentication\n  type: http\n  scheme: hmac\n  direction: Orum -> customer endpoint (consumer verifies)\n  header: x-webhook-signature\n  algorithm: HMAC-SHA256\n  encoding: base64\n  signed_value: '{timestamp}.{stringified_body}'\n  header_format: 't={timestamp},s={encoded-signature}'\n  key_management: >-\n    The signing key is chosen by the customer at webhook-creation time and typed into the Orum\n    UI. Orum does not generate it, does not rotate it,\
  \ and explicitly permits ignoring it:\n    \"you may discard it on receipt if you don't wish to use a signing key, but something does\n    need to be filled out here.\" There is no key rotation mechanism and no way to read the key\n    back out.\n  replay_protection: >-\n    Advisory only — Orum recommends rejecting payloads whose timestamp is more than five\n    minutes old. Not enforced by Orum.\n  standards_note: not RFC 9421 HTTP Message Signatures and not Standard Webhooks\n  source: https://support.orum.com/en-US/orum/article/ART-463-webhooks\n\ngaps:\n- No API authentication of any kind — no keys, no tokens, no OAuth client registration.\n- The Orum sign-in link on every page points at https://orum.com/oauth, which 404s to a plain\n  GET (unchanged since the 2026-08-04 pass) — the only \"auth\" URL Orum exposes publicly is\n  broken for anyone not arriving through the app.\n- Webhook signing keys are customer-supplied with no rotation, no strength requirement, and an\n  explicit\
  \ opt-out.\nx-evidence:\n  fetched: '2026-08-13'\n  probes:\n  - url: https://support.orum.com/en-US/orum/article/Am0DBxe--singlesignon-sso\n    status: 200\n  - url: https://support.orum.com/en-US/orum/article/ART-463-webhooks\n    status: 200\n  - url: https://orum.com/oauth\n    status: 404\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/orum-com/refs/heads/main/authentication/orum-com-authentication.yml
summary_line: saml/openIdConnect/oauth2/hmac-signature · 2 schemes
tags:
- Company
- AI
- Sales
- Sales Engagement
- Sales Dialer
- Outbound Sales
- Sales Coaching
- Conversation Intelligence
- Telephony
- Revenue Operations
- Webhooks
- Parallel Dialing
- Sales Automation
---
