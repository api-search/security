---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: silicon-box.com
  spf: true
hosts:
- cert_expires: Sep 16 10:35:50 2026 GMT
  host: www.silicon-box.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Silicon Box Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Silicon Box, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Silicon Box
provider_slug: silicon-box
slug: silicon-box-domain-security
source_filename: silicon-box-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.silicon-box.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 10:35:50 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: silicon-box.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/silicon-box/refs/heads/main/security/silicon-box-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Semiconductors
- Chiplets
- Advanced Packaging
- Manufacturing
- Hardware
- Foundry
- Singapore
- Company
---
