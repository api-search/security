---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: blockspring.com
  spf: true
hosts:
- cert_expires: Oct  8 21:36:55 2026 GMT
  host: blockspring.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Blockspring Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Blockspring, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Blockspring
provider_slug: blockspring
slug: blockspring-domain-security
source_filename: blockspring-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: blockspring.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 21:36:55 2026 GMT\n  hsts: false\ndomains:\n- domain: blockspring.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/blockspring/refs/heads/main/security/blockspring-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Data
- Integration
- Enrichment
- Spreadsheets
- Data Services
- Retired
---
