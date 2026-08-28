---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: searched
name: Mursion Authentication
name_suffix: Authentication
oauth_flows: []
overview: Mursion declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: Mursion
provider_slug: mursion
scheme_count: 0
schemes: []
slug: mursion-authentication
source_filename: mursion-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: searched\nsource: https://support.mursion.com/knowledge/configuring-an-sso-for-mursion\ndocs:\n- https://support.mursion.com/knowledge/configuring-an-sso-for-mursion\n- https://support.mursion.com/knowledge/configuring-saml-2.0\n- https://support.mursion.com/knowledge/configuring-saml-2.0-with-okta\n- https://support.mursion.com/knowledge/configuring-saml-2.0-with-microsoft-azure-ad\n- https://support.mursion.com/knowledge/configuring-saml-with-microsoft-entra-id\n- https://support.mursion.com/knowledge/configuring-openid-connect-with-okta\n- https://support.mursion.com/knowledge/team-assignment-via-sso\n- https://support.mursion.com/knowledge/frequently-asked-questions-about-single-sign-on-for-account-owners\nsummary: >-\n  Mursion publishes no public API reference and no machine-readable contract, so there is no\n  documented API authentication scheme (no API keys, no OAuth client credentials, no published\n  token endpoint). The authentication\
  \ surface Mursion DOES document publicly is enterprise\n  end-user identity federation into the Mursion Portal: SAML 2.0 and OpenID Connect, configured\n  per tenant by an account owner, with just-in-time user provisioning. This artifact records that\n  surface. Everything under apiaws.mursion.com — the REST backend the Mursion Portal SPA calls —\n  is gated: every probed path returns HTTP 403 {\"message\":\"Missing Authentication Token\"} from\n  AWS API Gateway.\napi_authentication:\n  documented: false\n  schemes: []\n  note: >-\n    No published API key, bearer token, OAuth client-credentials or mTLS scheme was found on any\n    Mursion host or in the customer knowledge base.\nuser_authentication:\n  documented: true\n  default: Email and password against the Mursion Portal, with optional TOTP second factor\n    (the portal exposes /profile/validateTotp/ and /profile/resend/otp).\n  federation:\n  - protocol: SAML 2.0\n    role: Mursion is the Service Provider (SP)\n    docs: https://support.mursion.com/knowledge/configuring-saml-2.0\n\
  \    flows:\n    - SP-initiated SSO\n    provisioning: JIT (Just In Time) — learner accounts are created on first successful login\n    sp_metadata: >-\n      Downloaded as an XML \"SP Metadata\" file from the Mursion Portal SSO configuration screen\n      once a configuration is created; it carries the Assertion Consumer Service URL. Mursion\n      does not publish a static, tenant-independent metadata URL.\n    idp_inputs:\n    - Single Sign-On Service Endpoint (IdP login URL)\n    - Logout Endpoint (IdP logout URL)\n    - Entity ID (IdP Issuer)\n    - X.509 certificate, PEM encoded\n    nameid_format: urn:oasis:names:tc:SAML:1.1:nameid-format:unspecified\n    required_attributes:\n    - name: email\n      purpose: user email address, the account key\n    - name: firstName\n      purpose: given name\n    - name: lastName\n      purpose: family name\n    optional_attributes:\n    - name: (configurable — \"Team Claim Name\")\n      purpose: >-\n        External team assignment; the claim\
  \ value maps the user onto a Mursion team.\n      docs: https://support.mursion.com/knowledge/team-assignment-via-sso\n    verified_idps:\n    - Okta\n    - Microsoft Entra ID\n    - Microsoft Azure AD\n  - protocol: OpenID Connect\n    role: Mursion is the Relying Party (RP)\n    docs: https://support.mursion.com/knowledge/configuring-openid-connect-with-okta\n    flows:\n    - SP-initiated SSO\n    - IdP-initiated SSO\n    provisioning: JIT (Just In Time)\n    scopes:\n    - openid\n    - profile\n    - email\n    claims:\n    - claim: sub\n      maps_to: user id\n    - claim: email\n      maps_to: email\n    - claim: given_name\n      maps_to: first name\n    - claim: family_name\n      maps_to: last name\n    - claim: (configurable — \"Team Claim Name\")\n      maps_to: team assignment\n      required: false\n    idp_inputs:\n    - Authorization endpoint\n    - Token endpoint\n    - User Info endpoint\n    - Logout endpoint\n    - Client ID and Client Secret\n    example_idp: >-\n\
  \      Okta — https://${yourOktaDomain}/oauth2/v1/authorize, /oauth2/v1/token,\n      /oauth2/v1/userinfo, /login/signout. These are the CUSTOMER's Okta endpoints, not\n      Mursion-operated endpoints.\n    verified_idps:\n    - Okta\n  discovery:\n    openid_configuration: >-\n      Not served by Mursion. /.well-known/openid-configuration returns 404 on www.mursion.com,\n      404 on support.mursion.com, 403 on apiaws.mursion.com, and an SPA HTML shell (200) on\n      portal.mursion.com. Mursion is the relying party; the discovery document belongs to the\n      customer's IdP.\nmarketplace_listings:\n- name: Okta Integration Network — Mursion\n  url: https://www.okta.com/integrations/mursion/\n  capabilities:\n  - SAML 2.0 SSO\ngaps:\n- No public API reference, therefore no documented API authentication model.\n- No published static SP metadata URL — SP metadata is per-tenant and downloaded from the portal.\n- No SCIM provisioning endpoint documented; user lifecycle is JIT-on-login plus\
  \ bulk import\n  (the portal exposes /import/sso-users and /import/non-sso-users to account owners).\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mursion/refs/heads/main/authentication/mursion-authentication.yml
summary_line: 0 schemes
tags:
- Company
- Learning and Development
- Corporate Training
- Simulation
- Immersive Learning
- Artificial Intelligence
- Virtual Reality
- Education
- Human Resources
- Enterprise Software
---
