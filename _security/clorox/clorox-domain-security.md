---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: clorox.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: thecloroxcompany.com
  spf: true
hosts:
- cert_expires: Oct 16 03:48:37 2026 GMT
  host: www.clorox.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 22 22:40:23 2026 GMT
  host: www.thecloroxcompany.com
  hsts: true
  hsts_max_age: 31622400
  https: true
  tls_version: TLSv1.3
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: Clorox Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for The Clorox Company, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: The Clorox Company
provider_slug: clorox
slug: clorox-domain-security
source_filename: clorox-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.clorox.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 16 03:48:37 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: www.thecloroxcompany.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 22 22:40:23 2026 GMT\n  hsts: true\n  hsts_max_age: 31622400\ndomains:\n- domain: clorox.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: thecloroxcompany.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/clorox/refs/heads/main/security/clorox-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Cleaning Products
- Consumer Goods
- CPG
- Disinfectants
- Household Products
- Manufacturer
- Fortune 500
- Safety Data Sheets
- Product Transparency
- MuleSoft
---
