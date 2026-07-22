---
api_key_in: []
auth_types:
- soap-auth-token
- preauth
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Zimbra Authentication
name_suffix: Authentication
oauth_flows: []
overview: Zimbra secures its APIs with soap-auth-token, preauth, and oauth2 across 4 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Zimbra
provider_slug: zimbra
scheme_count: 4
schemes:
- description: A SOAP <AuthRequest> in the urn:zimbraAccount namespace exchanges account name + password for an authToken, returned in the response and passed on subsequent requests via the <context><authToken> SOAP header (or the ZM_AUTH_TOKEN cookie for the web client).
  name: AuthRequest
  sources:
  - https://files.zimbra.com/docs/soap_api/
  type: soap-auth-token
- description: Pre-authentication (preauth) computes an HMAC-SHA1 over account/timestamp/expiry using a domain preauth key, enabling delegated/single-sign-on login without the account password.
  name: preauth
  sources:
  - https://wiki.zimbra.com/wiki/Preauth
  type: preauth
- description: Admin operations authenticate via <AuthRequest> in the urn:zimbraAdmin namespace against the admin SOAP endpoint (default port 7071 /service/admin/soap).
  name: admin-auth
  sources:
  - https://files.zimbra.com/docs/soap_api/
  type: soap-auth-token
- description: Two-factor authentication (TOTP) is supported; a second AuthRequest supplies the TOTP code when 2FA is enabled on the account.
  name: two-factor
  sources:
  - https://wiki.zimbra.com/wiki/Two_Factor_Authentication
  type: totp
slug: zimbra-authentication
source_filename: zimbra-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://files.zimbra.com/docs/soap_api/\ndocs: https://wiki.zimbra.com/wiki/SOAP_API_Reference_Material_Beginning_with_ZCS_8.0\nsummary:\n  types: [soap-auth-token, preauth, oauth2]\n  api_key_in: []\n  notes: Zimbra has no public OpenAPI; auth is documented in the SOAP API reference.\nschemes:\n- name: AuthRequest\n  type: soap-auth-token\n  description: A SOAP <AuthRequest> in the urn:zimbraAccount namespace exchanges account\n    name + password for an authToken, returned in the response and passed on subsequent\n    requests via the <context><authToken> SOAP header (or the ZM_AUTH_TOKEN cookie for\n    the web client).\n  sources: [https://files.zimbra.com/docs/soap_api/]\n- name: preauth\n  type: preauth\n  description: Pre-authentication (preauth) computes an HMAC-SHA1 over account/timestamp/expiry\n    using a domain preauth key, enabling delegated/single-sign-on login without the\n    account password.\n  sources: [https://wiki.zimbra.com/wiki/Preauth]\n\
  - name: admin-auth\n  type: soap-auth-token\n  description: Admin operations authenticate via <AuthRequest> in the urn:zimbraAdmin\n    namespace against the admin SOAP endpoint (default port 7071 /service/admin/soap).\n  sources: [https://files.zimbra.com/docs/soap_api/]\n- name: two-factor\n  type: totp\n  description: Two-factor authentication (TOTP) is supported; a second AuthRequest supplies\n    the TOTP code when 2FA is enabled on the account.\n  sources: [https://wiki.zimbra.com/wiki/Two_Factor_Authentication]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zimbra/refs/heads/main/authentication/zimbra-authentication.yml
summary_line: soap-auth-token/preauth/oauth2 · 4 schemes
tags:
- Email
- Collaboration
- Calendar
- Messaging
- Open Source
- SOAP
- GraphQL
- Productivity
---
