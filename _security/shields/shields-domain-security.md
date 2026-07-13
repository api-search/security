---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: shields.io
  spf: true
hosts:
- cert_expires: Sep  1 07:48:26 2026 GMT
  host: shields.io
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Shields Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Shields, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC absent.'
provider_name: Shields
provider_slug: shields
slug: shields-domain-security
source_filename: shields-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: shields.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  1 07:48:26 2026 GMT\n  hsts: false\ndomains:\n- domain: shields.io\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/shields/refs/heads/main/security/shields-domain-security.yml
summary_line: TLSv1.3 · DNSSEC
tags:
- Open Source Projects
- Public APIs
---
