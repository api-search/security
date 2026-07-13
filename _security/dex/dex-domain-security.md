---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: dexidp.io
  spf: false
hosts:
- cert_expires: Oct  4 22:48:32 2026 GMT
  host: dexidp.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Dex Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Dex, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Dex
provider_slug: dex
slug: dex-domain-security
source_filename: dex-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: dexidp.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 22:48:32 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: dexidp.io\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dex/refs/heads/main/security/dex-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Authentication
- Connectors
- Federation
- gRPC
- Identity Provider
- LDAP
- OAuth 2.0
- OIDC
- OpenID Connect
- SAML
- Single Sign-On
- SSO
---
