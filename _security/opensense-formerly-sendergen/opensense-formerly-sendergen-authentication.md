---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: searched
name: Opensense Formerly Sendergen Authentication
name_suffix: Authentication
oauth_flows: []
overview: Opensense (formerly SenderGen) declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: Opensense (formerly SenderGen)
provider_slug: opensense-formerly-sendergen
scheme_count: 3
schemes:
- applies_to: Opensense web application sign-in (app.opensense.com / accounts.opensense.com)
  id: saml-sso
  note: '"Opensense fully supports SAML 2.0 for secure and seamless integration with your identity provider. Contact your account manager for more information!"'
  providers:
  - Okta
  - SAP
  - Oracle
  - OneLogin
  - Ping Identity
  source: https://help.opensense.com/docs/opensense-supports-saml.md
  spec: SAML 2.0
  type: saml
- applies_to: Non-SSO Opensense user sign-in
  id: password
  scheme: password
  source: https://help.opensense.com/docs/update-your-password.md
  type: http
- applies_to: Opensense REST API / Zapier integration
  id: api-key
  issuance: manual
  note: '"Enter your domain and the Zapier API key. An Opensense integration specialist can provide you an API key if you don''t already have one." The key''s transport (header vs query parameter), name, format, rotation policy and expiry are not published.'
  self_service: false
  source: https://help.opensense.com/docs/zapier-integration.md
  transport: undocumented
  type: apiKey
slug: opensense-formerly-sendergen-authentication
source_filename: opensense-formerly-sendergen-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: >-\n  https://help.opensense.com/docs/opensense-supports-saml.md,\n  https://help.opensense.com/docs/zapier-integration.md,\n  https://help.opensense.com/docs/google-workspace-permissions.md,\n  https://help.opensense.com/docs/outreach-integration-permissions.md,\n  https://www.opensense.com/llms.txt\ndocs: https://help.opensense.com/docs/opensense-supports-saml.md\nsummary: >-\n  Opensense documents authentication for the PLATFORM, not for a public API.\n  Administrators sign in to app.opensense.com via SAML 2.0 SSO (or a password\n  for non-SSO users). A REST API is advertised on the marketing site and in\n  llms.txt, but the only publicly documented way to obtain a credential for it\n  is to ask an Opensense integration specialist for an API key — there is no\n  self-service key issuance, no developer portal, and no published token\n  endpoint. Derived scheme detail is unavailable because Opensense publishes no\n  OpenAPI\
  \ or other machine-readable contract.\nschemes:\n- id: saml-sso\n  type: saml\n  applies_to: Opensense web application sign-in (app.opensense.com / accounts.opensense.com)\n  spec: SAML 2.0\n  providers:\n  - Okta\n  - SAP\n  - Oracle\n  - OneLogin\n  - Ping Identity\n  note: >-\n    \"Opensense fully supports SAML 2.0 for secure and seamless integration with\n    your identity provider. Contact your account manager for more information!\"\n  source: https://help.opensense.com/docs/opensense-supports-saml.md\n- id: password\n  type: http\n  scheme: password\n  applies_to: Non-SSO Opensense user sign-in\n  source: https://help.opensense.com/docs/update-your-password.md\n- id: api-key\n  type: apiKey\n  applies_to: Opensense REST API / Zapier integration\n  issuance: manual\n  self_service: false\n  note: >-\n    \"Enter your domain and the Zapier API key. An Opensense integration\n    specialist can provide you an API key if you don't already have one.\" The\n    key's transport (header\
  \ vs query parameter), name, format, rotation policy\n    and expiry are not published.\n  transport: undocumented\n  source: https://help.opensense.com/docs/zapier-integration.md\nprovisioning:\n  scim: false\n  note: >-\n    User provisioning and de-provisioning is documented via Okta, and directory\n    sync from Azure AD / Entra ID, on-premise AD, Google Directory and Workday.\n    SCIM is not named by Opensense.\n  source: https://www.opensense.com/llms.txt\nconsumed_oauth_scopes:\n  note: >-\n    These are OAuth 2.0 scopes Opensense REQUESTS FROM third-party platforms as\n    an OAuth client. They are not scopes Opensense issues for its own API, so no\n    OAuthScopes pointer is emitted from them. Recorded because they are the only\n    published, itemised authorization surface this provider has.\n  providers:\n  - provider: Google Workspace\n    flow: OAuth 2.0 (Google Workspace Marketplace app \"Opensense (formerly SenderGen)\", publisher Opensense Inc.)\n    data_flow: one-way,\
  \ Google Workspace to Opensense\n    scopes:\n    - scope: https://www.googleapis.com/auth/admin.directory.user.readonly\n      access: read-only\n      purpose: Pull user attributes (name, title, department)\n    - scope: https://www.googleapis.com/auth/admin.directory.group.readonly\n      access: read-only\n      purpose: Identify group memberships to assign the correct signature template\n    - scope: https://www.googleapis.com/auth/admin.directory.orgunit.readonly\n      access: read-only\n      purpose: Filter or target based on the user's OU placement\n    - scope: https://www.googleapis.com/auth/gmail.settings.basic\n      access: read-write\n      purpose: Edit email signatures for the user's primary account\n    source: https://help.opensense.com/docs/google-workspace-permissions.md\n  - provider: Outreach\n    flow: OAuth 2.0, authorized by an Outreach administrator\n    scopes:\n    - scope: users.all\n      purpose: Read user profile data to populate and sync Opensense signature\
  \ fields\n    - scope: teams.read\n      purpose: Read team and group membership to assign users to Opensense groups\n    - scope: mailboxes.all\n      purpose: >-\n        Read and write Outreach mailbox settings to push the Opensense signature\n        block. Applies to Outreach mailbox records only; does not grant access to\n        the underlying Microsoft 365 / Google Workspace accounts.\n    - scope: prospects.read\n      purpose: Read prospect records to support recipient-based banner targeting\n    source: https://help.opensense.com/docs/outreach-integration-permissions.md\ngaps:\n- No public API reference or machine-readable specification\n- API key transport, format and rotation are undocumented\n- No self-service credential issuance; keys are requested from a human\n- No OAuth authorization server or OIDC discovery document is served on any Opensense host\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/opensense-formerly-sendergen/refs/heads/main/authentication/opensense-formerly-sendergen-authentication.yml
summary_line: 3 schemes
tags:
- Company
- Email Signature Management
- Email Marketing
- Brand Management
- Sales Enablement
- Marketing
- Email
---
