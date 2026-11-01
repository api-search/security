---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: p-1.ai
  spf: true
hosts:
- cert_expires: Dec 31 03:22:15 2026 GMT
  host: p-1.ai
  hsts: true
  hsts_max_age: 2630000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: P 1 Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for P-1, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: P-1
provider_slug: p-1
slug: p-1-domain-security
source_filename: p-1-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-22'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: p-1.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 31 03:22:15 2026 GMT\n  hsts: true\n  hsts_max_age: 2630000\ndomains:\n- domain: p-1.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/p-1/security/p-1-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- AI Engineering
- Mechanical Engineering
- Electrical Engineering
- Data Center Engineering
- Automotive
- Aerospace
- Defense
---
