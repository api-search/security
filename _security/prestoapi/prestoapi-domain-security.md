---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: prestoapi.com
  spf: true
hosts:
- cert_expires: Dec 31 13:14:00 2026 GMT
  host: prestoapi.com
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.2
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Prestoapi Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for PrestoAPI, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: PrestoAPI
provider_slug: prestoapi
slug: prestoapi-domain-security
source_filename: prestoapi-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: prestoapi.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec 31 13:14:00 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\ndomains:\n- domain: prestoapi.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/prestoapi/security/prestoapi-domain-security.yml
summary_line: TLSv1.2 · HSTS
tags:
- Company
- API Generation
- Data Integration
- Low-Code
- Automation
- Software-as-a-Service
---
