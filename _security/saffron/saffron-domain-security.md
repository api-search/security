---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: trysaffron.ai
  spf: false
hosts:
- cert_expires: Aug 22 15:45:11 2026 GMT
  host: www.trysaffron.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Saffron Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Saffron, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Saffron
provider_slug: saffron
slug: saffron-domain-security
source_filename: saffron-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.trysaffron.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 22 15:45:11 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: trysaffron.ai\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/saffron/refs/heads/main/security/saffron-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Hiring
- Technical Assessment
- Recruiting
- Artificial Intelligence
- Developer Tools
- Y Combinator
---
