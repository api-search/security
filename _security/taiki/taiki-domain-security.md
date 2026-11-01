---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: taiki.ai
  spf: true
hosts:
- cert_expires: Jan  4 12:36:04 2027 GMT
  host: taiki.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Taiki Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Taiki, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Taiki
provider_slug: taiki
slug: taiki-domain-security
source_filename: taiki-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: taiki.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  4 12:36:04 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: taiki.ai\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/taiki/security/taiki-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Tax Documents
- API
- Payroll Integration
- Financial Data Extraction
- Tax Forms
- Bank Statements
- Brokerage Statements
---
