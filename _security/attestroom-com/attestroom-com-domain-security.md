---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: attestroom.com
  spf: true
hosts:
- cert_expires: Dec  5 05:57:12 2026 GMT
  host: attestroom.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Attestroom Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for attestroom-com, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: attestroom-com
provider_slug: attestroom-com
slug: attestroom-com-domain-security
source_filename: attestroom-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: attestroom.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  5 05:57:12 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: attestroom.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/attestroom-com/security/attestroom-com-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Policy Management
- Compliance
- SaaS
- US
- Small Business
---
