---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: netstock.com
  spf: true
hosts:
- cert_expires: Dec 16 04:18:10 2026 GMT
  host: netstock.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Netstock Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Netstock, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Netstock
provider_slug: netstock
slug: netstock-domain-security
source_filename: netstock-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: netstock.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 16 04:18:10 2026 GMT\n  hsts: false\ndomains:\n- domain: netstock.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/netstock/security/netstock-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Supply Chain Planning
- Inventory Management
- Demand Planning
- AI
- ERP Integration
- Manufacturing
- Retail
- Wholesale
---
