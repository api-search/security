---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: lakridsbybulow.com
  spf: true
hosts:
- cert_expires: Sep  2 20:18:06 2026 GMT
  host: lakridsbybulow.com
  hsts: true
  hsts_max_age: 300
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Lakrids By B Low Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for LAKRIDS BY BÜLOW, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: LAKRIDS BY BÜLOW
provider_slug: lakrids-by-b-low
slug: lakrids-by-b-low-domain-security
source_filename: lakrids-by-b-low-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: lakridsbybulow.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  2 20:18:06 2026 GMT\n  hsts: true\n  hsts_max_age: 300\ndomains:\n- domain: lakridsbybulow.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lakrids-by-b-low/refs/heads/main/security/lakrids-by-b-low-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Consumer
- Consumer Goods
- Food and Beverage
- Confectionery
- Retail
- E-Commerce
- Denmark
---
