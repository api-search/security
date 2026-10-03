---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: biotia.io
  spf: true
hosts:
- cert_expires: Nov 24 06:29:40 2026 GMT
  host: biotia.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Biotia Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Biotia, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Biotia
provider_slug: biotia
slug: biotia-domain-security
source_filename: biotia-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: biotia.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 24 06:29:40 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: biotia.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/biotia/refs/heads/main/security/biotia-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Health Tech
- Diagnostics
- Infectious Diseases
- Biotechnology
- Company
---
