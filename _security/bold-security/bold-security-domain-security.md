---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: bold.security
  spf: true
hosts:
- cert_expires: Sep 30 10:29:40 2026 GMT
  host: www.bold.security
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Bold Security Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bold Security, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Bold Security
provider_slug: bold-security
slug: bold-security-domain-security
source_filename: bold-security-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.bold.security\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 10:29:40 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: bold.security\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bold-security/refs/heads/main/security/bold-security-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Ai Ml
- Data Security
- Endpoint Security
- Data Loss Prevention
- AI Security
- Cybersecurity
---
