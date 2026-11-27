---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: compslate.com
  spf: true
hosts:
- cert_expires: Apr  8 23:59:59 2027 GMT
  host: compslate.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: CompSlate Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CompSlate, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: CompSlate
provider_slug: compslate-com
slug: compslate-com-domain-security
source_filename: compslate-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: compslate.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Apr  8 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: compslate.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/compslate-com/security/compslate-com-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Sales Compensation
- Sales Commissions
- Revenue Operations
- MCP
- AI Assistant
- Software-as-a-Service
---
