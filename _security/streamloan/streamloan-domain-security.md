---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: streamloan.io
  spf: true
hosts:
- host: streamloan.io
  https: false
kind: domain-security
layout: security
method: probed
name: Streamloan Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for StreamLoan, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: StreamLoan
provider_slug: streamloan
slug: streamloan-domain-security
source_filename: streamloan-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: streamloan.io\n  https: false\ndomains:\n- domain: streamloan.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/streamloan/refs/heads/main/security/streamloan-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Company
- Mortgage
- Lending
- Loan Origination
- Point of Sale
- Fintech
- Real Estate
- SaaS
- Banking
- Financial Services
---
