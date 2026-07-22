---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: liquidly.com
  spf: false
hosts:
- cert_expires: Sep  6 23:26:43 2026 GMT
  host: www.liquidly.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Liquidly Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Liquidly, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Liquidly
provider_slug: liquidly
slug: liquidly-domain-security
source_filename: liquidly-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.liquidly.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  6 23:26:43 2026 GMT\n  hsts: false\ndomains:\n- domain: liquidly.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/liquidly/refs/heads/main/security/liquidly-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Financial Services
- Fintech
- Private Markets
- Secondary Market
- Alternative Assets
- Private Equity
- Venture Capital
- Marketplace
- Broker-Dealer
---
