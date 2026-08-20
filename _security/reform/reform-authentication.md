---
api_key_in: []
auth_types: []
description: Reform issues no API credentials. There is no public REST API, no developer portal, no API-key page, no OAuth authorization server and no OpenAPI securitySchemes to derive from — derive-authentication.py produced no profile because the repo holds no spec, and the help centre's only "API key" articles are about pasting THIRD-PARTY keys (Close CRM, Google reCAPTCHA) INTO Reform. The one credential Reform hands a developer is a per-webhook signing secret, used to verify inbound deliveries; it authenticates Reform to the customer, not the customer to Reform.
kind: authentication
layout: security
method: searched
name: Reform Authentication
name_suffix: Authentication
oauth_flows: []
overview: Reform declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: Reform
provider_slug: reform
scheme_count: 3
schemes:
- algorithm: HMAC-SHA256
  credential: per-webhook secret, retrieved from the dashboard (form → Integrations → Webhook → lock icon)
  direction: reform-to-customer
  docs: https://docs.reform.app/article/7-webhooks
  header: Signature
  id: webhook-hmac-signature
  note: This is the only cryptographic credential Reform gives a developer. It authenticates Reform's outbound webhook, it does NOT grant access to any Reform endpoint.
  type: message-signature
  verification: Recompute HMAC-SHA256 over the raw request body with the webhook secret and compare the hex digest to the Signature header. Reform publishes a PHP reference implementation.
- description: The headless-forms flow posts a plain HTML form to the Reform-generated form action on forms.reform.app with fields named answers[<block-id>]. No key, token or signature is involved; the form's own URL is the capability. Spam control is delegated to Google reCAPTCHA (the customer supplies their own Site Key/Secret) and to Reform's email-validation and free-email-provider blocking features.
  direction: customer-to-reform
  docs: https://docs.reform.app/article/15-using-your-own-html-form
  id: unauthenticated-form-post
  type: none
- description: Human login to the Reform application. Reform's security page states MFA is required for Reform employees and that strong passwords are required for platform users; no customer-facing SSO/SAML or MFA feature is documented in the help centre, and no OIDC discovery document is served (see well-known/reform-well-known.yml).
  endpoint: https://dashboard.reform.app/login
  id: dashboard-session
  type: interactive-login
slug: reform-authentication
source_filename: reform-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-14'\nmethod: searched\nsource: https://docs.reform.app/article/7-webhooks\ndocs:\n  - https://docs.reform.app/article/7-webhooks\n  - https://docs.reform.app/article/65-close\n  - https://docs.reform.app/article/38-how-to-set-up-google-recaptcha-integration\n  - https://docs.reform.app/article/15-using-your-own-html-form\ndescription: >-\n  Reform issues no API credentials. There is no public REST API, no developer\n  portal, no API-key page, no OAuth authorization server and no OpenAPI\n  securitySchemes to derive from — derive-authentication.py produced no profile\n  because the repo holds no spec, and the help centre's only \"API key\" articles\n  are about pasting THIRD-PARTY keys (Close CRM, Google reCAPTCHA) INTO Reform.\n  The one credential Reform hands a developer is a per-webhook signing secret,\n  used to verify inbound deliveries; it authenticates Reform to the customer,\n  not the customer to Reform.\napi_credentials_issued: false\noauth2: false\n\
  openid_connect: false\nmutual_tls: false\nschemes:\n  - id: webhook-hmac-signature\n    type: message-signature\n    direction: reform-to-customer\n    algorithm: HMAC-SHA256\n    header: Signature\n    credential: per-webhook secret, retrieved from the dashboard (form → Integrations → Webhook → lock icon)\n    verification: >-\n      Recompute HMAC-SHA256 over the raw request body with the webhook secret\n      and compare the hex digest to the Signature header. Reform publishes a PHP\n      reference implementation.\n    docs: https://docs.reform.app/article/7-webhooks\n    note: >-\n      This is the only cryptographic credential Reform gives a developer. It\n      authenticates Reform's outbound webhook, it does NOT grant access to any\n      Reform endpoint.\n  - id: unauthenticated-form-post\n    type: none\n    direction: customer-to-reform\n    description: >-\n      The headless-forms flow posts a plain HTML form to the Reform-generated\n      form action on forms.reform.app with\
  \ fields named answers[<block-id>].\n      No key, token or signature is involved; the form's own URL is the\n      capability. Spam control is delegated to Google reCAPTCHA (the customer\n      supplies their own Site Key/Secret) and to Reform's email-validation and\n      free-email-provider blocking features.\n    docs: https://docs.reform.app/article/15-using-your-own-html-form\n  - id: dashboard-session\n    type: interactive-login\n    endpoint: https://dashboard.reform.app/login\n    description: >-\n      Human login to the Reform application. Reform's security page states MFA\n      is required for Reform employees and that strong passwords are required\n      for platform users; no customer-facing SSO/SAML or MFA feature is\n      documented in the help centre, and no OIDC discovery document is served\n      (see well-known/reform-well-known.yml).\nthird_party_credentials_stored:\n  - {integration: Close CRM, credential: Close API key, note: generated in Close, pasted into Reform}\n\
  \  - {integration: Google reCAPTCHA, credential: Site Key + Site Secret, note: generated in the reCAPTCHA admin panel, pasted into Reform}\n  - {integration: HubSpot / ConvertKit (Kit) / Notion / Google Sheets / Slack, credential: OAuth or account connection performed inside the Reform dashboard, note: mechanics not documented publicly}\ngaps:\n  - No published API key, token, or OAuth flow for programmatic access to Reform data.\n  - No /.well-known/openid-configuration or /.well-known/oauth-authorization-server on any Reform host (all 404 or 403).\n  - No documented rotation policy, expiry, or scope model for the webhook signing secret.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/reform/refs/heads/main/authentication/reform-authentication.yml
summary_line: 3 schemes
tags:
- Forms
- Form Builder
- Lead Generation
- Headless Forms
- Webhook
- No-Code
- Integration
- CRM
- Conversion Rate Optimization
- Embeddable Components
---
