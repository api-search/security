---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: koreanpulse.dev
  spf: true
hosts:
- cert_expires: Jan 27 09:13:17 2027 GMT
  host: koreanpulse.dev
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: koreanpulse Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for koreanpulse, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: koreanpulse
provider_slug: koreanpulse-dev
slug: koreanpulse-dev-domain-security
source_filename: koreanpulse-dev-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-14'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: koreanpulse.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 27 09:13:17 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: koreanpulse.dev\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/koreanpulse-dev/security/koreanpulse-dev-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Korean
- Stocks
- Markets
- Artificial Intelligence
- Data
---
