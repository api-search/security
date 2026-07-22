---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: trdata.com
  spf: true
hosts:
- cert_expires: Aug 18 06:33:50 2026 GMT
  host: trdata.com
  hsts: true
  hsts_max_age: 604800
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Trdata Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for TRDATA, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: TRDATA
provider_slug: trdata
slug: trdata-domain-security
source_filename: trdata-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: trdata.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Aug 18 06:33:50 2026 GMT\n  hsts: true\n  hsts_max_age: 604800\ndomains:\n- domain: trdata.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/trdata/refs/heads/main/security/trdata-domain-security.yml
summary_line: TLSv1.2 · HSTS
tags:
- Company
- Financial Services
- Market Data
- Fixed Income
- OTC Markets
- Trading
- News
- Analytics
- Emerging Markets
- Bonds
---
