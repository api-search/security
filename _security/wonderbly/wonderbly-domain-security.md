---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: wonderbly.com
  spf: true
hosts:
- cert_expires: Jan  9 21:00:20 2027 GMT
  host: wonderbly.com
  hsts: true
  hsts_max_age: 31557600
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Wonderbly Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Wonderbly *, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Wonderbly *
provider_slug: wonderbly
slug: wonderbly-domain-security
source_filename: wonderbly-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: wonderbly.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  9 21:00:20 2027 GMT\n  hsts: true\n  hsts_max_age: 31557600\ndomains:\n- domain: wonderbly.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wonderbly/refs/heads/main/security/wonderbly-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Consumer
- E-commerce
- Personalization
- Publishing
- Books
- Gifts
- Retail
---
