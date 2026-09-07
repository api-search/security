---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: wyattcorp.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: drforhair.co.kr
  spf: false
hosts:
- cert_expires: Nov 28 15:02:28 2026 GMT
  host: wyattcorp.com
  hsts: false
  https: true
  tls_version: TLSv1.2
- cert_expires: Nov  9 15:32:08 2026 GMT
  host: drforhair.co.kr
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar 12 23:59:59 2027 GMT
  host: drforhair2024.cafe24api.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Wyatt Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Wyatt, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.2); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Wyatt
provider_slug: wyatt
slug: wyatt-domain-security
source_filename: wyatt-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: wyattcorp.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov 28 15:02:28 2026 GMT\n  hsts: false\n- host: drforhair.co.kr\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  9 15:32:08 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: drforhair2024.cafe24api.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 12 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: wyattcorp.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: drforhair.co.kr\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wyatt/refs/heads/main/security/wyatt-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Company
- Beauty
- Personal Care
- Haircare
- Consumer Products
- E-Commerce
- Retail
- Agentic Commerce
- Model Context Protocol
- South Korea
---
