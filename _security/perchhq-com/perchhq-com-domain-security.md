---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: perchhq.io
  spf: true
hosts:
- cert_expires: Dec 15 21:29:25 2026 GMT
  host: perchhq.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Perchhq Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Perch, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Perch
provider_slug: perchhq-com
slug: perchhq-com-domain-security
source_filename: perchhq-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: perchhq.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 15 21:29:25 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: perchhq.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/perchhq-com/security/perchhq-com-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Real Estate
- SaaS
- Digital Brochures
- Marketing
- Realtors
---
