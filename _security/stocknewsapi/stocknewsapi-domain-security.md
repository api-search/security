---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: stocknewsapi.com
  spf: true
hosts:
- cert_expires: Dec 14 16:55:41 2026 GMT
  host: stocknewsapi.com
  hsts: false
  https: true
  tls_version: TLSv1.2
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Stocknewsapi Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for StockNewsAPI, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: StockNewsAPI
provider_slug: stocknewsapi
slug: stocknewsapi-domain-security
source_filename: stocknewsapi-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: stocknewsapi.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec 14 16:55:41 2026 GMT\n  hsts: false\ndomains:\n- domain: stocknewsapi.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/stocknewsapi/refs/heads/main/security/stocknewsapi-domain-security.yml
summary_line: TLSv1.2
tags:
- Company
- Finance
- News
- Stocks
- Market Data
---
