---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: locofy.ai
  spf: true
hosts:
- cert_expires: Oct 30 23:59:59 2026 GMT
  host: www.locofy.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- host: builder.locofy.ai
  https: false
kind: domain-security
layout: security
method: probed
name: Locofy Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Locofy, probed live across 2 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Locofy
provider_slug: locofy
slug: locofy-domain-security
source_filename: locofy-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.locofy.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 30 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: builder.locofy.ai\n  https: false\ndomains:\n- domain: locofy.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/locofy/refs/heads/main/security/locofy-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Design to Code
- Figma
- Adobe XD
- Frontend
- AI Code Generation
- Low-Code
---
