---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: faldaro.app
  spf: false
hosts:
- cert_expires: Dec  8 17:17:39 2026 GMT
  host: faldaro.app
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Faldaro Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Faldaro, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Faldaro
provider_slug: faldaro-app
slug: faldaro-app-domain-security
source_filename: faldaro-app-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-07'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: faldaro.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  8 17:17:39 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: faldaro.app\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/faldaro-app/security/faldaro-app-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- SSO
- Claims Intake
---
