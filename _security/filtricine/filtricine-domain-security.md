---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: filtricine.com
  spf: true
hosts:
- cert_expires: Dec 13 06:57:24 2026 GMT
  host: filtricine.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Filtricine Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Filtricine, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Filtricine
provider_slug: filtricine
slug: filtricine-domain-security
source_filename: filtricine-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: filtricine.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 13 06:57:24 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: filtricine.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/filtricine/security/filtricine-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Biotechnology
- Cancer
- Medical-Food
- Clinical-Trials
- San-Francisco
---
