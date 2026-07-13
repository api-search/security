---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: awesomeapi.com.br
  spf: true
hosts:
- cert_expires: Aug 31 07:18:33 2026 GMT
  host: docs.awesomeapi.com.br
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Economia Awesome Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Economia.Awesome, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Economia.Awesome
provider_slug: economia-awesome
slug: economia-awesome-domain-security
source_filename: economia-awesome-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: docs.awesomeapi.com.br\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 31 07:18:33 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: awesomeapi.com.br\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/economia-awesome/refs/heads/main/security/economia-awesome-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Currency Exchange
- Public APIs
---
