---
api_key_in: []
auth_types: []
description: Blackstone publishes no public developer API and therefore no API key, bearer-token or developer OAuth programme. What it does serve anonymously is OpenID Connect discovery metadata from the two identity systems that gate its investor and documentation surfaces. This profile is derived entirely from those two fetched discovery documents plus the BXAccess portal's own unauthenticated runtime config. It describes how a HUMAN authenticates into Blackstone's gated surfaces — it does not describe a machine-to-machine API programme, because none is published.
kind: authentication
layout: security
method: probed
name: Blackstone Authentication
name_suffix: Authentication
oauth_flows: []
overview: Blackstone declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: Blackstone
provider_slug: blackstone
scheme_count: 0
schemes: []
slug: blackstone-authentication
source_filename: blackstone-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-10'\nmethod: probed\nsource: >-\n  https://auth.bx.com/identity-broker/.well-known/openid-configuration and\n  https://login.bx.com/.well-known/openid-configuration (both fetched 2026-08-10, HTTP 200)\nprovider: Blackstone\nproviderId: blackstone\ndescription: >-\n  Blackstone publishes no public developer API and therefore no API key, bearer-token or\n  developer OAuth programme. What it does serve anonymously is OpenID Connect discovery metadata\n  from the two identity systems that gate its investor and documentation surfaces. This profile\n  is derived entirely from those two fetched discovery documents plus the BXAccess portal's own\n  unauthenticated runtime config. It describes how a HUMAN authenticates into Blackstone's\n  gated surfaces — it does not describe a machine-to-machine API programme, because none is\n  published.\nsummary:\n  public_api_authentication: none-published\n  identity_protocol: OpenID Connect / OAuth 2.0\n  identity_providers:\
  \ 2\n  self_service_registration: false\n  api_keys_issued: false\nsecuritySchemes:\n  - name: bxaccess_oidc\n    type: openIdConnect\n    protocol: OpenID Connect 1.0\n    issuer: https://auth.bx.com\n    openIdConnectUrl: https://auth.bx.com/identity-broker/.well-known/openid-configuration\n    applies_to: BXAccess investor portal (https://www.bxaccess.com)\n    endpoints:\n      authorization: https://auth.bx.com/oauth2/authorize\n      token: https://auth.bx.com/oauth2/token\n      userinfo: https://auth.bx.com/oauth2/userInfo\n      revocation: https://auth.bx.com/oauth2/revoke\n      end_session: https://auth.bx.com/logout\n      jwks: https://auth.bx.com/identity-broker/.well-known/jwks.json\n    response_types_supported:\n      - code\n      - token\n    token_endpoint_auth_methods_supported:\n      - client_secret_basic\n      - client_secret_post\n    id_token_signing_alg_values_supported:\n      - RS256\n    scopes_supported:\n      - openid\n      - email\n      - phone\n \
  \     - profile\n    client_registration: closed\n    notes: >-\n      The portal's public runtime config at https://www.bxaccess.com/bxa-next/env.json declares\n      a single fixed public client and the scope string \"openid email profile\". There is no\n      dynamic client registration endpoint on this issuer, so no third party can obtain a client\n      here. PKCE is not advertised in this discovery document.\n  - name: bx_okta_oidc\n    type: openIdConnect\n    protocol: OpenID Connect 1.0\n    issuer: https://login.bx.com\n    openIdConnectUrl: https://login.bx.com/.well-known/openid-configuration\n    applies_to: >-\n      Firmwide Blackstone SSO; observed gating docs.blackstone.com through the GitBook VA-Okta\n      visitor-auth integration\n    endpoints:\n      authorization: https://login.bx.com/oauth2/v1/authorize\n      token: https://login.bx.com/oauth2/v1/token\n      userinfo: https://login.bx.com/oauth2/v1/userinfo\n      introspection: https://login.bx.com/oauth2/v1/introspect\n\
  \      revocation: https://login.bx.com/oauth2/v1/revoke\n      end_session: https://login.bx.com/oauth2/v1/logout\n      registration: https://login.bx.com/oauth2/v1/clients\n      jwks: https://login.bx.com/oauth2/v1/keys\n    grant_types_supported:\n      - authorization_code\n      - implicit\n      - refresh_token\n      - password\n      - 'urn:ietf:params:oauth:grant-type:device_code'\n      - 'urn:openid:params:grant-type:ciba'\n    code_challenge_methods_supported:\n      - S256\n    token_endpoint_auth_methods_supported:\n      - client_secret_basic\n      - client_secret_post\n      - client_secret_jwt\n      - private_key_jwt\n      - none\n    id_token_signing_alg_values_supported:\n      - RS256\n    id_token_encryption_alg_values_supported:\n      - RSA-OAEP-256\n      - RSA-OAEP-384\n      - RSA-OAEP-512\n    scopes_supported:\n      - openid\n      - email\n      - profile\n      - address\n      - phone\n      - offline_access\n      - groups\n    client_registration:\
  \ >-\n      A dynamic client registration endpoint is advertised (Okta default). It was NOT exercised —\n      this pipeline does not create clients on a provider's tenant.\n    notes: >-\n      Standard Okta org tenant on a custom domain (login.bx.com CNAMEs to\n      bx.customdomains.okta.com). PKCE with S256 is supported.\ngated_surfaces:\n  - surface: https://docs.blackstone.com\n    gate: GitBook VA-Okta visitor-auth → login.bx.com\n    observed_status: 307 on every path\n  - surface: https://www.bxaccess.com\n    gate: OIDC login against auth.bx.com/identity-broker\n    observed_status: 302 to /auth/login on every unauthenticated path\n  - surface: https://bxnexus.my.site.com/BlackstoneAdvantagePortal/s/login/\n    gate: Salesforce Experience Cloud community login (Blackstone Advantage Portal for advisors)\n    observed_status: referenced from the BXAccess bundle; login-walled\n  - surface: https://mdm.blackstone.com/DataManagement\n    gate: WS-Federation SSO with wtrealm=https://www.bxaccess.com/\n\
  \    observed_status: 403 (Cloudflare managed challenge) to non-browser clients\nmaintainers:\n  - FN: Kin Lane\n    email: kin@apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/blackstone/refs/heads/main/authentication/blackstone-authentication.yml
summary_line: 0 schemes
tags:
- Alternative Assets
- Finance
- Investment Management
- Private Equity
- Real Estate
- Fortune 500
---
