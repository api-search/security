---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: kaavio.ai
  spf: true
hosts:
- cert_expires: Sep  4 00:23:05 2026 GMT
  host: kaavio.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Kaavio Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Kaavio, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Kaavio
provider_slug: kaavio
slug: kaavio-domain-security
source_filename: kaavio-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: kaavio.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  4 00:23:05 2026 GMT\n  hsts: null\ndomains:\n- domain: kaavio.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kaavio/refs/heads/main/security/kaavio-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Product Content
- Product Data
- Product Information Management
- PIM
- Catalog Management
- B2B Distribution
- Manufacturing
- E-commerce
- Artificial Intelligence
- Content Generation
- Data Enrichment
---
