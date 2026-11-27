---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: innernote.space
  spf: true
hosts:
- cert_expires: Jan  2 11:12:21 2027 GMT
  host: innernote.space
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: innernote Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for innernote, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: innernote
provider_slug: innernote-space
slug: innernote-space-domain-security
source_filename: innernote-space-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: innernote.space\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  2 11:12:21 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: innernote.space\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/innernote-space/security/innernote-space-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Software-as-a-Service
- Artificial Intelligence
- LinkedIn
- Content Generation
- Productivity
---
