---
api_specs:
- filename: sso-saml-openapi.yml
  format: yaml
  label: SAML SSO Authentication API
  slug: saml-authentication
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sso/refs/heads/main/openapi/sso-saml-openapi.yml
- filename: sso-oidc-openapi.yml
  format: yaml
  label: OpenID Connect (OIDC) Authentication API
  slug: oidc-authentication
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sso/refs/heads/main/openapi/sso-oidc-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: oasis-open.org
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: openid.net
  spf: true
hosts:
- cert_expires: Sep  3 09:37:11 2026 GMT
  host: www.oasis-open.org
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  5 11:30:22 2026 GMT
  host: openid.net
  hsts: true
  hsts_max_age: 31557600
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Sso Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SSO, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: SSO
provider_slug: sso
slug: sso-domain-security
source_filename: sso-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.oasis-open.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  3 09:37:11 2026 GMT\n  hsts: false\n- host: openid.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  5 11:30:22 2026 GMT\n  hsts: true\n  hsts_max_age: 31557600\ndomains:\n- domain: oasis-open.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: openid.net\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sso/refs/heads/main/security/sso-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Authentication
- Authorization
- Identity
- OAuth
- OIDC
- SAML
- Security
- Single Sign-On
- SSO
---
