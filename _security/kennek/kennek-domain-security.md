---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: kennek.io
  spf: true
hosts:
- cert_expires: Aug 26 19:01:20 2026 GMT
  host: kennek.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Kennek Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Kennek, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Kennek
provider_slug: kennek
slug: kennek-domain-security
source_filename: kennek-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: kennek.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 26 19:01:20 2026 GMT\n  hsts: null\ndomains:\n- domain: kennek.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kennek/refs/heads/main/security/kennek-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Fintech
- Lending
- Loan Management
- Loan Servicing
- Loan Origination
- Financial Services
- SaaS
---
