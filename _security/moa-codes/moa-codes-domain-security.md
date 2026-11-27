---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: moa.codes
  spf: true
hosts:
- cert_expires: Jan 16 04:55:35 2027 GMT
  host: moa.codes
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: moa Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for moa, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: moa
provider_slug: moa-codes
slug: moa-codes-domain-security
source_filename: moa-codes-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: moa.codes\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 16 04:55:35 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: moa.codes\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/moa-codes/security/moa-codes-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Artificial Intelligence
- Transcription
- Translation
- Meetings
---
