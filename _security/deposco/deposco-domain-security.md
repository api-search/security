---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: deposco.com
  spf: true
hosts:
- cert_expires: Aug 24 23:59:59 2026 GMT
  host: deposco.com
  hsts: false
  https: true
  tls_version: TLSv1.2
- cert_expires: Nov 10 23:59:59 2026 GMT
  host: developer.deposco.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Deposco Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Deposco, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Deposco
provider_slug: deposco
slug: deposco-domain-security
source_filename: deposco-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: deposco.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Aug 24 23:59:59 2026 GMT\n  hsts: false\n- host: developer.deposco.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 10 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: deposco.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/deposco/refs/heads/main/security/deposco-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- Supply Chain
- Warehouse Management
- WMS
- Order Management
- OMS
- Fulfillment
- Inventory
- Logistics
- Ecommerce
- 3PL
---
