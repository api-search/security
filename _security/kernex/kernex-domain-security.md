---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: kernex.io
  spf: true
hosts:
- cert_expires: Dec 31 13:27:06 2026 GMT
  host: kernex.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Kernex Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Kernex Limited, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Kernex Limited
provider_slug: kernex
slug: kernex-domain-security
source_filename: kernex-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: kernex.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 31 13:27:06 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: kernex.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/kernex/security/kernex-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Headless CMS
- Content Management
- API-First
- Cloud
---
