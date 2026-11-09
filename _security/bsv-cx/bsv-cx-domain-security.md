---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: bsv.cx
  spf: true
hosts:
- cert_expires: Jan 10 04:06:45 2027 GMT
  host: bsv.cx
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Bsv Cx Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for bsv.cx, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: bsv.cx
provider_slug: bsv-cx
slug: bsv-cx-domain-security
source_filename: bsv-cx-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: bsv.cx\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 10 04:06:45 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: bsv.cx\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/bsv-cx/security/bsv-cx-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Bitcoin
- Timestamping
- Blockchain
- Verification
- Trustless
---
