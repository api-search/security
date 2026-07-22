---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: kimberly-clark.com
  spf: true
hosts:
- cert_expires: Aug 17 21:28:17 2026 GMT
  host: www.kimberly-clark.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Kimberly Clark Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Kimberly-Clark, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Kimberly-Clark
provider_slug: kimberly-clark
slug: kimberly-clark-domain-security
source_filename: kimberly-clark-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.kimberly-clark.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 17 21:28:17 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: kimberly-clark.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kimberly-clark/refs/heads/main/security/kimberly-clark-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Consumer Goods
- Consumer Products
- Fortune 500
- Personal Care
- Tissue
---
