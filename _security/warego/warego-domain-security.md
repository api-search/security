---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: warego.co
  spf: true
hosts:
- cert_expires: Oct 18 09:08:45 2026 GMT
  host: warego.co
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Warego Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for WareGo, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: WareGo
provider_slug: warego
slug: warego-domain-security
source_filename: warego-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: warego.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 18 09:08:45 2026 GMT\n  hsts: false\ndomains:\n- domain: warego.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/warego/refs/heads/main/security/warego-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Warehouse Management
- WMS
- Inventory Management
- Order Management
- Fulfillment
- Supply Chain
- Logistics
- 3PL
- Ecommerce
- Retail
- Wholesale Distribution
- Manufacturing
- EDI
---
