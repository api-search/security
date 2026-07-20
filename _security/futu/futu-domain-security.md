---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: futuholdings.com
  spf: true
hosts:
- cert_expires: Oct 11 23:59:59 2026 GMT
  host: futuholdings.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Futu Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Futu, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Futu
provider_slug: futu
slug: futu-domain-security
source_filename: futu-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: futuholdings.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 11 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: futuholdings.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/futu/refs/heads/main/security/futu-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Technology
- FinTech
- Brokerage
- Trading
- Market Data
- Stocks
- Options
- Investing
- Financial Services
---
