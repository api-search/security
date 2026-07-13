---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: racinghub.net
  spf: false
hosts:
- cert_expires: Aug 26 11:47:41 2026 GMT
  host: racinghub.net
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Racinghub Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for RacingHub, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: RacingHub
provider_slug: racinghub
slug: racinghub-domain-security
source_filename: racinghub-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: racinghub.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 26 11:47:41 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: racinghub.net\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/racinghub/refs/heads/main/security/racinghub-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Sports And Fitness
- Public APIs
---
