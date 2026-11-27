---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: frtracker.app
  spf: true
hosts:
- cert_expires: Dec 26 00:01:57 2026 GMT
  host: frtracker.app
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Federal Regulatory Tracker Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Federal Regulatory Tracker, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Federal Regulatory Tracker
provider_slug: frtracker-app
slug: frtracker-app-domain-security
source_filename: frtracker-app-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-08'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: frtracker.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 26 00:01:57 2026 GMT\n  hsts: null\ndomains:\n- domain: frtracker.app\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/frtracker-app/security/frtracker-app-domain-security.yml
summary_line: TLSv1.3
tags:
- Regulatory Research
- Data Services
- Federal Register
---
