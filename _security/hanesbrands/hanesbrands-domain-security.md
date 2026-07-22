---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: hanesbrands.com
  spf: true
hosts:
- cert_expires: Aug 25 14:29:54 2026 GMT
  host: www.hanesbrands.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Hanesbrands Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Hanesbrands, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Hanesbrands
provider_slug: hanesbrands
slug: hanesbrands-domain-security
source_filename: hanesbrands-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.hanesbrands.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 25 14:29:54 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: hanesbrands.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hanesbrands/refs/heads/main/security/hanesbrands-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Apparel
- Consumer Goods
- Retail
- Fortune 500
---
