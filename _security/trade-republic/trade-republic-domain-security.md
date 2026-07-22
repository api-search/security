---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: traderepublic.com
  spf: true
hosts:
- cert_expires: Jan 16 23:59:59 2027 GMT
  host: traderepublic.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Trade Republic Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Trade Republic, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Trade Republic
provider_slug: trade-republic
slug: trade-republic-domain-security
source_filename: trade-republic-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: traderepublic.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 16 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: traderepublic.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/trade-republic/refs/heads/main/security/trade-republic-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Consumer
- FinTech
- Trading
- Investing
- Banking
- Savings
- Brokerage
- Europe
---
