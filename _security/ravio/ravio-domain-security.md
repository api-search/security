---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: ravio.com
  spf: true
hosts:
- cert_expires: Sep 29 18:44:33 2026 GMT
  host: ravio.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ravio Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ravio, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Ravio
provider_slug: ravio
slug: ravio-domain-security
source_filename: ravio-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ravio.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 18:44:33 2026 GMT\n  hsts: null\ndomains:\n- domain: ravio.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ravio/refs/heads/main/security/ravio-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Enterprise
- Compensation
- Benchmarking
- Total Rewards
- Human Resources
- HR Tech
- SaaS
---
