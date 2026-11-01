---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: adoptclarity.com
  spf: true
hosts:
- cert_expires: Dec 27 02:35:44 2026 GMT
  host: www.adoptclarity.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Adoptclarity Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Clarity, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Clarity
provider_slug: adoptclarity-com
slug: adoptclarity-com-domain-security
source_filename: adoptclarity-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.adoptclarity.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 27 02:35:44 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: adoptclarity.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/adoptclarity-com/security/adoptclarity-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- AI
- Meeting-Transcription
- Productivity
- Sales
---
