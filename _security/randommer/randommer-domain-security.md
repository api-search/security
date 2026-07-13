---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: randommer.io
  spf: false
hosts:
- cert_expires: Aug 13 04:44:29 2026 GMT
  host: randommer.io
  hsts: true
  hsts_max_age: 7776000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Randommer Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Randommer, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Randommer
provider_slug: randommer
slug: randommer-domain-security
source_filename: randommer-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: randommer.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 13 04:44:29 2026 GMT\n  hsts: true\n  hsts_max_age: 7776000\ndomains:\n- domain: randommer.io\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/randommer/refs/heads/main/security/randommer-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Test Data
- Public APIs
---
