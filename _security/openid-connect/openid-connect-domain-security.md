---
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
name: Openid Connect Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for OpenID Connect, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: OpenID Connect
provider_slug: openid-connect
slug: openid-connect-domain-security
source_filename: openid-connect-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: openid.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  5 11:30:22 2026 GMT\n  hsts: true\n  hsts_max_age: 31557600\ndomains:\n- domain: openid.net\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/openid-connect/refs/heads/main/security/openid-connect-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Authentication
- Identity
- JWT
- OAuth
- OpenID Connect
---
