---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: cmgx.io
  spf: true
hosts:
- cert_expires: Oct 10 15:53:24 2026 GMT
  host: cmgx.io
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Capital Markets Gateway Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Capital Markets Gateway, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Capital Markets Gateway
provider_slug: capital-markets-gateway
slug: capital-markets-gateway-domain-security
source_filename: capital-markets-gateway-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-09'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cmgx.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 10 15:53:24 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: cmgx.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/capital-markets-gateway/refs/heads/main/security/capital-markets-gateway-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Financial-Services
- Capital Markets
- Equity Capital Markets
- Market Data
- Data Intelligence
- Workflow Management
- Investment Banking
- Fintech
---
