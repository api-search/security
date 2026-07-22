---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: secretescapes.com
  spf: true
hosts:
- cert_expires: Feb  7 23:59:59 2027 GMT
  host: secretescapes.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Secret Escapes Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Secret Escapes, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Secret Escapes
provider_slug: secret-escapes
slug: secret-escapes-domain-security
source_filename: secret-escapes-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: secretescapes.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Feb  7 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: secretescapes.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/secret-escapes/refs/heads/main/security/secret-escapes-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Company
- Consumer
- Travel
- Hospitality
- E-commerce
- Membership
- Flash Sales
---
