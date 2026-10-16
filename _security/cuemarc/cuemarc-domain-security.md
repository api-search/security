---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: cuemarc.com
  spf: true
hosts:
- cert_expires: Nov 19 16:05:22 2026 GMT
  host: cuemarc.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Cuemarc Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cuemarc, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Cuemarc
provider_slug: cuemarc
slug: cuemarc-domain-security
source_filename: cuemarc-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-16'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cuemarc.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 19 16:05:22 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: cuemarc.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cuemarc/refs/heads/main/security/cuemarc-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- AI
- Reputation-Management
- Marketing
- LLM
---
