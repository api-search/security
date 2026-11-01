---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: toteminsights.com
  spf: false
hosts:
- cert_expires: Jan 12 11:40:21 2027 GMT
  host: toteminsights.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Toteminsights Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Humanitru, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Humanitru
provider_slug: toteminsights-com
slug: toteminsights-com-domain-security
source_filename: toteminsights-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-24'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: toteminsights.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan 12 11:40:21 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: toteminsights.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/toteminsights-com/security/toteminsights-com-domain-security.yml
summary_line: TLSv1.2 · HSTS
tags:
- Company
- CRM
- Nonprofit
- Data Integration
- Donor Management
---
