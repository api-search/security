---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: getfrenchie.dev
  spf: true
hosts:
- cert_expires: Jan 12 17:57:58 2027 GMT
  host: getfrenchie.dev
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: LAB94 Co., Ltd. Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for LAB94 Co., Ltd., probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: LAB94 Co., Ltd.
provider_slug: getfrenchie-dev
slug: getfrenchie-dev-domain-security
source_filename: getfrenchie-dev-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-09'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: getfrenchie.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 12 17:57:58 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: getfrenchie.dev\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/getfrenchie-dev/security/getfrenchie-dev-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Artificial Intelligence
- Tools
- OCR
- Transcription
- Content Extraction
---
