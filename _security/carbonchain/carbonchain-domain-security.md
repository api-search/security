---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: carbonchain.com
  spf: true
hosts:
- cert_expires: Aug 22 07:42:13 2026 GMT
  host: www.carbonchain.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Carbonchain Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CarbonChain, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: CarbonChain
provider_slug: carbonchain
slug: carbonchain-domain-security
source_filename: carbonchain-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.carbonchain.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 22 07:42:13 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: carbonchain.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/carbonchain/refs/heads/main/security/carbonchain-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Carbon Accounting
- Emissions Tracking
- Supply Chain
- Heavy Industry
- Commodities
- Metals And Mining
- Manufacturing
- CBAM
- Scope 3 Emissions
- Product Carbon Footprint
- Sustainability
- ESG
- Climate
- Regulatory Compliance
- CSRD
- CDP
---
