---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: quizapi.io
  spf: true
hosts:
- cert_expires: Sep  9 22:52:49 2026 GMT
  host: quizapi.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Quizapi Io Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for quizapi.io, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: quizapi.io
provider_slug: quizapi-io
slug: quizapi-io-domain-security
source_filename: quizapi-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: quizapi.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  9 22:52:49 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: quizapi.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/quizapi-io/refs/heads/main/security/quizapi-io-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Games And Comics
- Public APIs
---
