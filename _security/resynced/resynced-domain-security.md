---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: resynced.io
  spf: true
hosts:
- cert_expires: Nov 28 23:41:03 2026 GMT
  host: resynced.io
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Resynced Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for LeanyLabs, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: LeanyLabs
provider_slug: resynced
slug: resynced-domain-security
source_filename: resynced-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: resynced.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 28 23:41:03 2026 GMT\n  hsts: null\ndomains:\n- domain: resynced.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/resynced/security/resynced-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Data Integration
- APIs
- Automation
- Cloud Services
---
