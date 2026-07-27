---
api_key_in:
- header
auth_types:
- http
- hmac
description: The Vodafone Business Messaging Hub API authenticates with account-scoped API keys minted in the console — there is no OAuth 2.0, no OpenID Connect, no CIBA and no mutual TLS anywhere on the TPG Telecom developer surface. Anonymous probes of the OAuth/OIDC discovery documents on api.messaging.tpgtelecom.com.au return 404.
kind: authentication
layout: security
method: searched
name: Tpg Telecom Authentication
name_suffix: Authentication
oauth_flows: []
overview: TPG Telecom secures its APIs with http and hmac across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: TPG Telecom
provider_slug: tpg-telecom
scheme_count: 3
schemes:
- description: 'Authorization: Basic Base64(api_key:api_secret). The API key and secret are issued from the Messaging Hub console (Settings > API Settings > Basic Authentication).'
  docs: https://support.messaging.tpgtelecom.com.au/hc/en-us/articles/4750274170383-Creating-new-API-credentials
  header: Authorization
  name: BasicAuth
  scheme: basic
  sources:
  - blueprint/tpg-telecom-contacts-management-api.apib
  type: http
- algorithm: hmac-sha1
  description: 'Authorization: hmac username="<API KEY>", algorithm="hmac-sha1", headers="Date Content-MD5 request-line", signature="<SIGNATURE>". Requests without a body omit Content-MD5 and sign headers="Date request-line".'
  docs: https://support.messaging.tpgtelecom.com.au/hc/en-us/articles/4750274170383-Creating-new-API-credentials
  name: HmacAuth
  scheme: hmac
  signing:
    body_digest_header: Content-MD5 (MD5 of the request body; omitted when no body)
    date_header: Date (RFC 7231 section 7.1.1.2 format)
    signature: Base64(HMAC-SHA1(signing string, api_secret))
    signing_string: Date header, Content-MD5 header (when set) and the request line joined by line breaks
  sources:
  - blueprint/tpg-telecom-contacts-management-api.apib
  type: http
- description: Legacy username/password API credentials, created in the console under Settings > API Settings > Legacy API Credentials. The help centre describes these as the credentials used to "connect with your Sinch MessageMedia account".
  name: LegacyCredentials
  scheme: basic
  sources:
  - https://support.messaging.tpgtelecom.com.au/hc/en-us/articles/4750274170383-Creating-new-API-credentials
  status: legacy
  type: http
slug: tpg-telecom-authentication
source_filename: tpg-telecom-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-25'\nmethod: searched\nsource: >-\n  blueprint/tpg-telecom-contacts-management-api.apib (Authentication section) plus the\n  Vodafone Business Messaging Hub help-centre articles \"Creating new API credentials\"\n  and \"Managing Existing API Credentials\".\ndocs: https://support.messaging.tpgtelecom.com.au/hc/en-us/articles/4750274170383-Creating-new-API-credentials\ndescription: >-\n  The Vodafone Business Messaging Hub API authenticates with account-scoped API keys\n  minted in the console — there is no OAuth 2.0, no OpenID Connect, no CIBA and no\n  mutual TLS anywhere on the TPG Telecom developer surface. Anonymous probes of the\n  OAuth/OIDC discovery documents on api.messaging.tpgtelecom.com.au return 404.\nsummary:\n  types: [http, hmac]\n  api_key_in: [header]\n  oauth2_flows: []\n  oauth2: false\n  oidc: false\n  mtls: false\n  ciba: false\nschemes:\n- name: BasicAuth\n  type: http\n  scheme: basic\n  description: >-\n    Authorization: Basic Base64(api_key:api_secret).\
  \ The API key and secret are issued\n    from the Messaging Hub console (Settings > API Settings > Basic Authentication).\n  header: Authorization\n  sources:\n  - blueprint/tpg-telecom-contacts-management-api.apib\n  docs: https://support.messaging.tpgtelecom.com.au/hc/en-us/articles/4750274170383-Creating-new-API-credentials\n- name: HmacAuth\n  type: http\n  scheme: hmac\n  algorithm: hmac-sha1\n  description: >-\n    Authorization: hmac username=\"<API KEY>\", algorithm=\"hmac-sha1\", headers=\"Date\n    Content-MD5 request-line\", signature=\"<SIGNATURE>\". Requests without a body omit\n    Content-MD5 and sign headers=\"Date request-line\".\n  signing:\n    date_header: Date (RFC 7231 section 7.1.1.2 format)\n    body_digest_header: Content-MD5 (MD5 of the request body; omitted when no body)\n    signing_string: Date header, Content-MD5 header (when set) and the request line joined by line breaks\n    signature: Base64(HMAC-SHA1(signing string, api_secret))\n  sources:\n  - blueprint/tpg-telecom-contacts-management-api.apib\n\
  \  docs: https://support.messaging.tpgtelecom.com.au/hc/en-us/articles/4750274170383-Creating-new-API-credentials\n- name: LegacyCredentials\n  type: http\n  scheme: basic\n  status: legacy\n  description: >-\n    Legacy username/password API credentials, created in the console under Settings >\n    API Settings > Legacy API Credentials. The help centre describes these as the\n    credentials used to \"connect with your Sinch MessageMedia account\".\n  sources:\n  - https://support.messaging.tpgtelecom.com.au/hc/en-us/articles/4750274170383-Creating-new-API-credentials\ncredential_issuance:\n  self_serve: false\n  who: Account Administrators only (Basic and Advanced account permissions cannot manage keys)\n  where: Messaging Hub console — Settings > API Settings\n  secret_visibility: The API secret is displayed exactly once at creation; a lost secret requires a new key/secret pair.\n  rotation: Keys are created, renamed and deleted from the same console screen.\n  docs:\n  - https://support.messaging.tpgtelecom.com.au/hc/en-us/articles/4750274170383-Creating-new-API-credentials\n\
  \  - https://support.messaging.tpgtelecom.com.au/hc/en-us/articles/4750458066959-Managing-Existing-API-Credentials\naccount_security:\n  two_factor: https://support.messaging.tpgtelecom.com.au/hc/en-us/articles/5576504931343-2FA-Two-Factor-Authentication\n  sso: https://support.messaging.tpgtelecom.com.au/hc/en-us/articles/4694345111823-SSO-Single-sign-on-configuration\n  roles: https://support.messaging.tpgtelecom.com.au/hc/en-us/articles/4693954167695-User-roles\n  best_practices: https://support.messaging.tpgtelecom.com.au/hc/en-us/articles/4694325372047-Best-practices-for-securing-your-account\n  note: >-\n    2FA and SSO protect the console (human) login, not API calls; the API itself has no\n    scope model — a key carries the permissions of the account it belongs to.\nprobes:\n- url: https://api.messaging.tpgtelecom.com.au/.well-known/openid-configuration\n  status: 404\n- url: https://api.messaging.tpgtelecom.com.au/.well-known/oauth-authorization-server\n  status: 404\n- url:\
  \ https://api.messaging.tpgtelecom.com.au/.well-known/oauth-protected-resource\n  status: 404\n- url: https://api.messaging.tpgtelecom.com.au/api/v1/contacts/contacts\n  status: 401\n  body: '{\"message\":\"Unauthorized\"}'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tpg-telecom/refs/heads/main/authentication/tpg-telecom-authentication.yml
summary_line: http/hmac · 3 schemes
tags:
- Telecommunications
- Australia
- Mobile Network Operator
- Broadband
- Messaging
- SMS
- IoT
- 5G
- Partner Gated
---
