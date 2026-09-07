---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: aak.com
  spf: true
hosts:
- cert_expires: Oct 22 13:51:21 2026 GMT
  host: www.aak.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Aak Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AAK, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: AAK
provider_slug: aak
slug: aak-domain-security
source_filename: aak-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.aak.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 22 13:51:21 2026 GMT\n  hsts: false\ndomains:\n- domain: aak.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aak/refs/heads/main/security/aak-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Food and Beverage
- Ingredients
- Vegetable Oils
- Fats
- Manufacturing
- Chemicals
- Consumer Goods
- Agriculture
- Sweden
---
