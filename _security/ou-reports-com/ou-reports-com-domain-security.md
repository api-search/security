---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: ou-reports.com
  spf: true
hosts:
- cert_expires: Dec 25 02:09:54 2026 GMT
  host: ou-reports.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.2
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: OU Reports Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for OU Reports, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: OU Reports
provider_slug: ou-reports-com
slug: ou-reports-com-domain-security
source_filename: ou-reports-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ou-reports.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec 25 02:09:54 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: ou-reports.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/ou-reports-com/security/ou-reports-com-domain-security.yml
summary_line: TLSv1.2 · HSTS
tags:
- Macro‑Intelligence
- Live Events
- Qlik Migration
---
