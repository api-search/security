---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: descartes.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: macropoint.com
  spf: true
hosts:
- cert_expires: Nov 15 23:59:59 2026 GMT
  host: www.descartes.com
  hsts: true
  hsts_max_age: 300
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 19 07:24:44 2026 GMT
  host: docs.macropoint.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb  2 23:59:59 2027 GMT
  host: macropoint-lite.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Descartes Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Descartes Systems Group, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Descartes Systems Group
provider_slug: descartes
slug: descartes-domain-security
source_filename: descartes-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.descartes.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 15 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 300\n- host: docs.macropoint.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 19 07:24:44 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: macropoint-lite.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  2 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: descartes.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: macropoint.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/descartes/refs/heads/main/security/descartes-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Logistics
- Supply Chain
- Freight Visibility
- Shipment Tracking
- Customs Compliance
- Global Trade
- Trade Content
- Carrier Sourcing
---
