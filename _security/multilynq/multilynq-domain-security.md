---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: multilynq.com
  spf: true
hosts:
- cert_expires: Nov  5 19:28:42 2026 GMT
  host: www.multilynq.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Multilynq Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for MultiLynq, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: MultiLynq
provider_slug: multilynq
slug: multilynq-domain-security
source_filename: multilynq-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.multilynq.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  5 19:28:42 2026 GMT\n  hsts: false\ndomains:\n- domain: multilynq.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/multilynq/refs/heads/main/security/multilynq-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Fixed Income
- Bond Trading
- Capital Markets
- Financial Services
- Market Data
- Trading Connectivity
- FinTech
- API Integration
---
