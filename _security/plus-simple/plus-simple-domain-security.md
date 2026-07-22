---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: plussimple.com
  spf: true
hosts:
- cert_expires: Sep 29 10:47:34 2026 GMT
  host: plussimple.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Plus Simple Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Plus Simple, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Plus Simple
provider_slug: plus-simple
slug: plus-simple-domain-security
source_filename: plus-simple-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: plussimple.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 10:47:34 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: plussimple.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/plus-simple/refs/heads/main/security/plus-simple-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Insurance
- Insurtech
- Fintech
- Brokerage
- Underwriting
- France
- B2B
---
