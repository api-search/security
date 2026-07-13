---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: flexe.com
  spf: true
hosts:
- cert_expires: Aug 17 20:56:33 2026 GMT
  host: www.flexe.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  3 15:27:05 2026 GMT
  host: developer-sandbox.flexe.com
  hsts: false
  https: true
  tls_version: TLSv1.2
- cert_expires: Oct  3 15:27:05 2026 GMT
  host: api.flexe.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Flexe Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Flexe, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Flexe
provider_slug: flexe
slug: flexe-domain-security
source_filename: flexe-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.flexe.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 17 20:56:33 2026 GMT\n  hsts: false\n- host: developer-sandbox.flexe.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct  3 15:27:05 2026 GMT\n  hsts: false\n- host: api.flexe.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct  3 15:27:05 2026 GMT\n  hsts: null\ndomains:\n- domain: flexe.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/flexe/refs/heads/main/security/flexe-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Warehousing
- Logistics
- Fulfillment
- Supply Chain
- Inventory
- On-Demand
---
