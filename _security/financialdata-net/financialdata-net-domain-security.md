---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: financialdata.net
  spf: true
hosts:
- cert_expires: Sep 29 04:12:35 2026 GMT
  host: financialdata.net
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Financialdata Net Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for FinancialData.Net, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: FinancialData.Net
provider_slug: financialdata-net
slug: financialdata-net-domain-security
source_filename: financialdata-net-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-22'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: financialdata.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 04:12:35 2026 GMT\n  hsts: false\ndomains:\n- domain: financialdata.net\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/financialdata-net/refs/heads/main/security/financialdata-net-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- finance
- financial-data
- stock-market-api
- market-data
- equities
- etf
- crypto
- forex
- derivatives-options
- fundamentals
- insider-trading
- institutional-13f
- esg
- economic-data
- mcp
- investing
- trading
---
