---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: markr.ai
  spf: false
hosts:
- cert_expires: Jan  8 23:59:27 2027 GMT
  host: markr.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Markr Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Markr, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Markr
provider_slug: markr
slug: markr-domain-security
source_filename: markr-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: markr.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  8 23:59:27 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: markr.ai\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/markr/refs/heads/main/security/markr-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- AI
- Machine Learning
- Consulting
- Services
---
