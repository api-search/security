---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: weedmaps.com
  spf: true
hosts:
- cert_expires: Mar 26 21:00:27 2027 GMT
  host: weedmaps.com
  hsts: true
  hsts_max_age: 60
  https: true
  tls_version: TLSv1.2
- cert_expires: Aug 16 19:33:53 2026 GMT
  host: developer.weedmaps.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar 26 21:00:27 2027 GMT
  host: api-g.weedmaps.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Weedmaps Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Weedmaps, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.2); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Weedmaps
provider_slug: weedmaps
slug: weedmaps-domain-security
source_filename: weedmaps-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: weedmaps.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Mar 26 21:00:27 2027 GMT\n  hsts: true\n  hsts_max_age: 60\n- host: developer.weedmaps.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 16 19:33:53 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api-g.weedmaps.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Mar 26 21:00:27 2027 GMT\n  hsts: null\ndomains:\n- domain: weedmaps.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/weedmaps/refs/heads/main/security/weedmaps-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Cannabis
- Dispensary
- Marketplace
- Menu Sync
- Point of Sale
- Orders
- Brands
- Partner API
---
