---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: hopstack.io
  spf: true
hosts:
- cert_expires: Aug 17 04:03:27 2026 GMT
  host: www.hopstack.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 27 23:59:59 2026 GMT
  host: apidocs.hopstack.io
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Hopstack Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Hopstack, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Hopstack
provider_slug: hopstack
slug: hopstack-domain-security
source_filename: hopstack-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.hopstack.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 17 04:03:27 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: apidocs.hopstack.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 27 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: hopstack.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hopstack/refs/heads/main/security/hopstack-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Warehouse Management
- WMS
- Fulfillment
- Logistics
- Supply Chain
- Inventory
- 3PL
- E-commerce
---
