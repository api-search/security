---
api_specs:
- filename: oidc.yml
  format: yaml
  label: OpenID Connect API
  slug: openid-connect
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oidc/refs/heads/main/openapi/oidc.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: openid.net
  spf: true
hosts:
- cert_expires: Sep  5 11:30:22 2026 GMT
  host: openid.net
  hsts: true
  hsts_max_age: 31557600
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Oidc Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for OIDC, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: OIDC
provider_slug: oidc
slug: oidc-domain-security
source_filename: oidc-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: openid.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  5 11:30:22 2026 GMT\n  hsts: true\n  hsts_max_age: 31557600\ndomains:\n- domain: openid.net\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/oidc/refs/heads/main/security/oidc-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Authentication
- Identity
- JWT
- OAuth
- OIDC
- OpenID Connect
---
