---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: nanoparse.app
  spf: false
hosts:
- cert_expires: Jan  5 03:42:47 2027 GMT
  host: nanoparse.app
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Nanoparse Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for NanoParse, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF absent, DMARC present (p=none).'
provider_name: NanoParse
provider_slug: nanoparse
slug: nanoparse-domain-security
source_filename: nanoparse-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-15'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: nanoparse.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  5 03:42:47 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: nanoparse.app\n  dnssec: true\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nanoparse/refs/heads/main/security/nanoparse-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Web Parsing
- AI Agents
- Markdown Conversion
- Litmus Scoring
- Crypto Payments
---
