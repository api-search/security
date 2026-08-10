---
api_key_in:
- unspecified
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Steno Authentication
name_suffix: Authentication
oauth_flows: []
overview: Steno secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Steno
provider_slug: steno
scheme_count: 1
schemes:
- description: A confidential, organization-scoped API key. Steno generates one key per customer organization on request — the Litify guide instructs the customer to send Steno their 18-digit Salesforce Organization ID, and Steno returns the key. The key and the Steno API URL are then stored in the Salesforce "Steno Configuration" Custom Metadata Type (separate records for Staging and Production), not in a Named Credential.
  environments:
  - name: Staging
    note: separate Custom Metadata record
  - name: Production
    note: separate Custom Metadata record
  in: unspecified
  issuance: contact Steno (concierge@steno.com or the account manager) with the tenant organization ID
  name: StenoApiKey
  rotation_policy: not published
  sources:
  - https://help.steno.com/steno-litify-integration
  - https://help.steno.com/litify/how-to-retrieve-your-18-digit-org-id
  type: apiKey
slug: steno-authentication
source_filename: steno-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-05'\nmethod: searched\nsource: https://help.steno.com/steno-litify-integration\ndocs: https://help.steno.com/steno-litify-integration\nnote: 'Derived mechanically from OpenAPI is not possible — Steno publishes no specification.\n  This profile is read from the only public documentation of Steno API credentials:\n  the Steno-Litify Salesforce installation guide.'\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - unspecified\n  oauth2_flows: []\n  scopes_published: false\n  spec_backed: false\nschemes:\n- name: StenoApiKey\n  type: apiKey\n  in: unspecified\n  description: 'A confidential, organization-scoped API key. Steno generates one key\n    per customer organization on request — the Litify guide instructs the customer\n    to send Steno their 18-digit Salesforce Organization ID, and Steno returns the\n    key. The key and the Steno API URL are then stored in the Salesforce \"Steno Configuration\"\n    Custom Metadata Type (separate records for Staging\
  \ and Production), not in a Named\n    Credential.'\n  issuance: contact Steno (concierge@steno.com or the account manager) with the tenant\n    organization ID\n  rotation_policy: not published\n  sources:\n  - https://help.steno.com/steno-litify-integration\n  - https://help.steno.com/litify/how-to-retrieve-your-18-digit-org-id\n  environments:\n  - name: Staging\n    note: separate Custom Metadata record\n  - name: Production\n    note: separate Custom Metadata record\nend_user_authentication:\n  note: These are the human sign-in controls for Steno's own applications, not API\n    credentials. Recorded here because they are the only other published Steno auth\n    surface.\n  sign_in: https://steno.com/account/sign-in\n  controls:\n  - name: SAML Single Sign-On\n    docs: https://help.steno.com/setting-up-saml-single-sign-on-sso\n  - name: Multi-factor authentication\n    scope: Firm Dashboard\n    docs: https://help.steno.com/how-to-set-up-multi-factor-authentication-mfa-for-your-firm-dashboard\n\
  \  - name: Role-based access control\n    scope: Firm Dashboard\n    docs: https://help.steno.com/how-to-enable-role-based-access-control\n  - name: Firm Dashboard user roles and access control\n    docs: https://help.steno.com/firm-dashboard-access-control\ngaps:\n- No public API reference documents the header or query parameter the API key travels\n  in.\n- No OAuth 2.0, OpenID Connect, or scope model is published for the integration API.\n- '/.well-known/openid-configuration and /.well-known/oauth-authorization-server are\n  404 on steno.com and 403 on api.steno.com.'\nx-evidence:\n- url: https://help.steno.com/steno-litify-integration\n  http_status: 200\n  observed: '\"The API Key is a confidential and unique key for your organization. If\n    you don''t have it yet, please send us your Organization ID, and we will generate\n    the key for you.\" Configured via Setup > Custom Metadata Types > Steno Configuration.'\n- url: https://help.steno.com/setting-up-saml-single-sign-on-sso\n\
  \  http_status: 200\n- url: https://api.steno.com/.well-known/openid-configuration\n  http_status: 403\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/steno/refs/heads/main/authentication/steno-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Legal
- Legal Technology
- Court Reporting
- Depositions
- Litigation Support
- Transcription
- Video
- Artificial Intelligence
- Salesforce
---
