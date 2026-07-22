---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: metycle.com
  spf: true
hosts:
- cert_expires: Mar  8 23:59:59 2027 GMT
  host: metycle.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Metycle Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for METYCLE, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: METYCLE
provider_slug: metycle
slug: metycle-domain-security
source_filename: metycle-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: metycle.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar  8 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: metycle.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/metycle/refs/heads/main/security/metycle-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Marketplace
- Metals
- Recycling
- Scrap Metal
- Commodities
- Circular Economy
- Sustainability
- B2B
- Trading
- Germany
---
