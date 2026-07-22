---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: clap.company
  spf: false
hosts:
- cert_expires: Sep 10 09:56:26 2026 GMT
  host: welcome.clap.company
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Clap Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CLAP, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=quarantine).'
provider_name: CLAP
provider_slug: clap
slug: clap-domain-security
source_filename: clap-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: welcome.clap.company\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 10 09:56:26 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: clap.company\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/clap/refs/heads/main/security/clap-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Human Resources
- Performance Management
- SaaS
- OKR
- Employee Feedback
- Artificial Intelligence
- South Korea
---
