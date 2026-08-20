---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: searched
name: Vrify Authentication
name_suffix: Authentication
oauth_flows: []
overview: VRIFY declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: VRIFY
provider_slug: vrify
scheme_count: 0
schemes: []
slug: vrify-authentication
source_filename: vrify-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-05'\nmethod: searched\nsource: https://help.vrify.com/en/articles/16101816-set-up-and-use-multi-factor-authentication\ndocs:\n- https://help.vrify.com/en/articles/16101816-set-up-and-use-multi-factor-authentication\n- https://help.vrify.com/en/articles/14307460-understanding-user-permissions-in-vrify\n- https://help.vrify.com/en/articles/12455609-add-update-or-remove-user-permissions-in-vrify\n- https://help.vrify.com/en/articles/12120448-switch-companies-in-your-vrify-account\n- https://help.vrify.com/en/articles/12316516-change-your-vrify-password-on-the-web\n\nsummary: >-\n  VRIFY publishes no public API and therefore no API authentication model — no\n  API keys, no OAuth client registration, no token endpoint, no developer\n  credentials of any kind. What it documents is END-USER authentication into the\n  VRIFY web app and iOS app. The one machine-facing scheme observed is the bearer\n  challenge on its own internal backend, which is not offered to\
  \ third parties.\n\napi_authentication:\n  public_api: false\n  schemes: []\n  observed:\n  - host: services.vrify.com\n    path: /v2/\n    scheme: http-bearer\n    challenge: 'WWW-Authenticate: Bearer realm=\"api\"'\n    body: '{\"detail\":\"Authentication credentials were not provided.\"}'\n    stack: Django REST Framework behind uvicorn (Wagtail-based \"VRIFY Internal Dashboard\")\n    documented: false\n    offered_to_third_parties: false\n    note: >-\n      Discovered by probing hosts found in certificate transparency, not from any\n      VRIFY documentation. Its interactive docs endpoint /v2/docs 302s to the\n      Django staff login at /admin/login/. Recorded as observed fact, not as a\n      developer-facing contract.\n\nend_user_authentication:\n  primary:\n    method: username-and-password\n    docs: https://help.vrify.com/en/articles/12316516-change-your-vrify-password-on-the-web\n  mfa:\n    supported: true\n    factor: email one-time code\n    enforced_on:\n    - VRIFY web\
  \ app\n    - VRIFY iOS app\n    controlled_by: Company Admin (Settings -> Security -> \"Require email verification codes\")\n    scope: org-wide toggle; when on, all users must enter a one-time code at login\n    rollout: >-\n      Gradual rollout as of the 2026 help-centre article; may not be enabled on\n      every account.\n    docs: https://help.vrify.com/en/articles/16101816-set-up-and-use-multi-factor-authentication\n  sso:\n    supported: true\n    type: social/enterprise identity providers (consumed, not issued)\n    providers:\n    - Google\n    - Microsoft\n    - LinkedIn\n    - Apple\n    mfa_interaction: >-\n      VRIFY's own email-OTP MFA does NOT apply to SSO accounts — identity is\n      verified by the SSO provider.\n    saml: not documented\n    scim: not documented\n    discovery_document: >-\n      None published. /.well-known/openid-configuration returns 404 on vrify.com,\n      admin.vrify.com and services.vrify.com — VRIFY is an OIDC relying party,\n      not a provider.\n\
  \  multi_tenancy:\n    supported: true\n    model: >-\n      A user account can belong to more than one company and switches between\n      them in-app on web and iOS.\n    docs: https://help.vrify.com/en/articles/12120448-switch-companies-in-your-vrify-account\n  authorization:\n    model: role + per-feature user permissions\n    admin_role: Company Admin\n    granularity: user-level permissions set per product area\n    docs: https://help.vrify.com/en/articles/14307460-understanding-user-permissions-in-vrify\n    machine_readable_scopes: false\n\noauth_scopes: null\noauth_scopes_note: >-\n  Not applicable — no OAuth 2.0 authorization server, no published scopes, and no\n  third-party application registration. scopes/ is deliberately not emitted.\n\ngaps:\n- No API keys, personal access tokens, or service accounts offered to customers.\n- No OAuth/OIDC provider metadata published on any VRIFY host.\n- No documented SAML or SCIM provisioning.\n- Permissions are described in prose only;\
  \ no machine-readable permission or scope reference.\n\nx-evidence:\n- url: https://help.vrify.com/en/articles/16101816-set-up-and-use-multi-factor-authentication.md\n  http_status: 200\n  fetched: '2026-08-05'\n- url: https://services.vrify.com/v2/\n  http_status: 401\n  fetched: '2026-08-05'\n- url: https://vrify.com/.well-known/openid-configuration\n  http_status: 404\n  fetched: '2026-08-05'\n- url: https://services.vrify.com/v2/docs\n  http_status: 302\n  fetched: '2026-08-05'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vrify/refs/heads/main/authentication/vrify-authentication.yml
summary_line: 0 schemes
tags:
- Company
- Mining
- Mineral Exploration
- Geoscience
- Artificial Intelligence
- Machine-Learning
- 3D Visualization
- Data Visualization
- Investor Relations
- Software-as-a-Service
- Canada
---
