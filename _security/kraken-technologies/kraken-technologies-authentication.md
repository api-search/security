---
api_key_in: []
auth_types:
- jwt-bearer
- saml
- sso
description: ''
kind: authentication
layout: security
method: searched
name: Kraken Technologies Authentication
name_suffix: Authentication
oauth_flows: []
overview: Kraken Technologies secures its APIs with jwt-bearer, saml, and sso across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Kraken Technologies
provider_slug: kraken-technologies
scheme_count: 3
schemes:
- bearerFormat: JWT
  claims:
  - description: ID of the Support User in Kraken who made the request via the app
    name: user_id
  - description: Email address of the Support User
    name: user_email
  - description: Issued-at time
    name: iat
  - description: Expiry — 25 hours after issue
    name: exp
  - description: Name of the app the request came from
    name: aud
  - description: Kraken App specific permissions the user has — documented as "(soon)", not yet present
    name: permissions
  description: A Kraken Embedded App is handed a JWT (`appProxyJwt`) at initialisation by the Kraken Apps framework. The app presents it on every request through the Kraken App Proxy, which validates it and forwards it to the app's own backend. The token is the proof that the request originated from a user logged into Kraken.
  key_discovery:
    jwks_uri_pattern: <kraken-host>/.well-known/jwks.json
    kid: kraken-app-store
    note: Per-tenant; Kraken publishes no tenant host list, so no JWKS document could be retrieved.
    probeable_anonymously: false
    published_on:
    - Supportsite domain of each Kraken deployment
    - the APIs of each Kraken deployment
    verbatim: '"Each Kraken publishes its public key in the /.well-known/jwks.json endpoint, both in its Supportsite domain, and its APIs. The public key has kid set to kraken-app-store."'
  name: kraken-app-proxy-jwt
  proxy_url_form: <APIProxyURL>/<your endpoint>  e.g. https://kraken-app-proxy.example.com/p/v1/example-app/external/endpoint/
  scheme: bearer
  scopes_published: 0
  source: https://github.com/kraken-tech/kraken-apps-examples
  surface: Kraken Apps (Embedded Apps) → Kraken App Store Proxy
  token_lifetime: 25h
  transport_headers:
  - name: X-Kraken-App-Proxy-Authorization
    required: true
    value: Bearer <appProxyJwt>
  - name: X-Kraken-App-Proxy-Destination
    note: The proxy has a single endpoint that forwards all requests to the declared destination.
    required: true
    value: <destination host, e.g. external.com>
  type: http
- anonymous_access: false
  description: The documentation portal is a Django application that gates every path behind /auth/login/?next=<path>. It offers "Log in via SSO" plus an ad-hoc email/password fallback at /auth/login/ad-hoc/. Credentials are issued to licensees and contracted partners only.
  name: kraken-docs-sso
  probe:
    date: '2026-07-27'
    location: /auth/login/?next=/
    server: gunicorn
    status: 302
    x_frame_options: DENY
  surface: docs.kraken.tech (reference documentation portal)
  type: sso
- description: '"Integration with client identity providers (IdPs) supporting Security Assertion Markup Language (SAML) for Kraken Customer Platform", with multi-factor authentication support across Kraken access points and role-based access control with regular privileged-access audits.'
  name: kraken-platform-idp-saml
  source: https://www.kraken.tech/legal/trust-center
  surface: Kraken Customer Platform (product sign-in, not the API)
  type: saml
slug: kraken-technologies-authentication
source_filename: kraken-technologies-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-27'\nmethod: searched\nsource: >-\n  https://github.com/kraken-tech/kraken-apps-examples (README + src/types/app.ts, retrieved\n  2026-07-27), https://www.kraken.tech/legal/trust-center, live probes of docs.kraken.tech\ndocs: https://github.com/kraken-tech/kraken-apps-examples#the-kraken-apps-jwt\nsummary:\n  types: [jwt-bearer, saml, sso]\n  api_key_in: []\n  oauth2_flows: []\n  openapi_derived: false\n  note: >-\n    There is no OpenAPI to derive securitySchemes from. Everything below was read from Kraken's own\n    public example repository and Trust Center. The Open Kraken REST/event API authentication scheme\n    is NOT published; the only concretely documented API auth mechanism is the Kraken Apps\n    (Embedded Apps) proxy JWT.\nschemes:\n- name: kraken-app-proxy-jwt\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  surface: Kraken Apps (Embedded Apps) → Kraken App Store Proxy\n  source: https://github.com/kraken-tech/kraken-apps-examples\n\
  \  description: >-\n    A Kraken Embedded App is handed a JWT (`appProxyJwt`) at initialisation by the Kraken Apps\n    framework. The app presents it on every request through the Kraken App Proxy, which validates it\n    and forwards it to the app's own backend. The token is the proof that the request originated\n    from a user logged into Kraken.\n  transport_headers:\n  - name: X-Kraken-App-Proxy-Authorization\n    value: 'Bearer <appProxyJwt>'\n    required: true\n  - name: X-Kraken-App-Proxy-Destination\n    value: '<destination host, e.g. external.com>'\n    required: true\n    note: The proxy has a single endpoint that forwards all requests to the declared destination.\n  proxy_url_form: '<APIProxyURL>/<your endpoint>  e.g. https://kraken-app-proxy.example.com/p/v1/example-app/external/endpoint/'\n  key_discovery:\n    jwks_uri_pattern: '<kraken-host>/.well-known/jwks.json'\n    kid: kraken-app-store\n    published_on: [Supportsite domain of each Kraken deployment, the APIs of\
  \ each Kraken deployment]\n    verbatim: >-\n      \"Each Kraken publishes its public key in the /.well-known/jwks.json endpoint, both in its\n      Supportsite domain, and its APIs. The public key has kid set to kraken-app-store.\"\n    probeable_anonymously: false\n    note: Per-tenant; Kraken publishes no tenant host list, so no JWKS document could be retrieved.\n  claims:\n  - {name: user_id, description: ID of the Support User in Kraken who made the request via the app}\n  - {name: user_email, description: Email address of the Support User}\n  - {name: iat, description: Issued-at time}\n  - {name: exp, description: Expiry — 25 hours after issue}\n  - {name: aud, description: Name of the app the request came from}\n  - {name: permissions, description: 'Kraken App specific permissions the user has — documented as \"(soon)\", not yet present'}\n  token_lifetime: 25h\n  scopes_published: 0\n- name: kraken-docs-sso\n  type: sso\n  surface: docs.kraken.tech (reference documentation portal)\n\
  \  description: >-\n    The documentation portal is a Django application that gates every path behind\n    /auth/login/?next=<path>. It offers \"Log in via SSO\" plus an ad-hoc email/password fallback at\n    /auth/login/ad-hoc/. Credentials are issued to licensees and contracted partners only.\n  probe:\n    date: '2026-07-27'\n    status: 302\n    location: '/auth/login/?next=/'\n    server: gunicorn\n    x_frame_options: DENY\n  anonymous_access: false\n- name: kraken-platform-idp-saml\n  type: saml\n  surface: Kraken Customer Platform (product sign-in, not the API)\n  source: https://www.kraken.tech/legal/trust-center\n  description: >-\n    \"Integration with client identity providers (IdPs) supporting Security Assertion Markup Language\n    (SAML) for Kraken Customer Platform\", with multi-factor authentication support across Kraken\n    access points and role-based access control with regular privileged-access audits.\nnot_published:\n  oauth2: >-\n    No OAuth 2.0 authorization\
  \ server, flows, client registration or scope model is published on any\n    public Kraken host. /.well-known/oauth-authorization-server and /.well-known/oauth-protected-\n    resource on docs.kraken.tech return the login page, not RFC 8414/9728 metadata.\n  openid_connect: >-\n    No anonymous OIDC discovery document is served. docs.kraken.tech/.well-known/openid-configuration\n    returns text/html (the login page) with HTTP 200.\n  api_keys: No API key format, header name or issuance process is documented publicly.\n  mutual_tls: >-\n    Not documented for API access. mTLS-style client certificates DO appear in Kraken's internal\n    toolchain (the public Homebrew formula passes HOMEBREW_SSL_CLIENT_CERT to Nexus), but that is\n    package distribution, not API authentication.\n  scopes: 0\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kraken-technologies/refs/heads/main/authentication/kraken-technologies-authentication.yml
summary_line: jwt-bearer/saml/sso · 3 schemes
tags:
- Energy
- United Kingdom
- Utilities
- Electricity
- Gas
- Smart Metering
- Demand Response
- DER
- Billing
- Energy Platform
---
