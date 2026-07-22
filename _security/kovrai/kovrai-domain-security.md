---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: kovr.ai
  spf: false
hosts:
- cert_expires: Oct  5 07:25:03 2026 GMT
  host: kovr.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Kovrai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Kovr.ai, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Kovr.ai
provider_slug: kovrai
slug: kovrai-domain-security
source_filename: kovrai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: kovr.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 07:25:03 2026 GMT\n  hsts: false\ndomains:\n- domain: kovr.ai\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kovrai/refs/heads/main/security/kovrai-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Compliance
- Security
- Governance
- Cloud
- Artificial Intelligence
- Risk
---
