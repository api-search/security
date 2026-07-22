---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: fintool.ai
  spf: true
hosts:
- cert_expires: Dec 19 11:22:29 2026 GMT
  host: fintool.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Fintool Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Fintool, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Fintool
provider_slug: fintool
slug: fintool-domain-security
source_filename: fintool-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: fintool.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 19 11:22:29 2026 GMT\n  hsts: null\ndomains:\n- domain: fintool.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fintool/refs/heads/main/security/fintool-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Financial Services
- Artificial Intelligence
- Equity Research
- Investment Research
- SEC Filings
- Fintech
- Large Language Models
---
