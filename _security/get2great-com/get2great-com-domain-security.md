---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: get2great.com
  spf: true
hosts:
- cert_expires: Dec  8 14:14:32 2026 GMT
  host: get2great.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Get2Great Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Get2Great, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Get2Great
provider_slug: get2great-com
slug: get2great-com-domain-security
source_filename: get2great-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-09'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: get2great.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  8 14:14:32 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: get2great.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/get2great-com/security/get2great-com-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Benchmarking
- Management
- Analytics
- Human Resources
- Software-as-a-Service
---
