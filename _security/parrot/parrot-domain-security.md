---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: parrot.us
  spf: true
hosts:
- cert_expires: Oct 16 01:01:32 2026 GMT
  host: parrot.us
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Parrot Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Parrot, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Parrot
provider_slug: parrot
slug: parrot-domain-security
source_filename: parrot-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: parrot.us\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 16 01:01:32 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: parrot.us\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/parrot/refs/heads/main/security/parrot-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Ai Ml
- Legal Tech
- Court Reporting
- Deposition
- Transcription
- Insurance
- Medical Records
- Litigation
---
