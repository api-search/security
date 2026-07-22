---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: pubmatic.com
  spf: true
hosts:
- cert_expires: Nov 21 23:59:59 2026 GMT
  host: pubmatic.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Pubmatic Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for PubMatic, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: PubMatic
provider_slug: pubmatic
slug: pubmatic-domain-security
source_filename: pubmatic-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: pubmatic.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 21 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: pubmatic.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pubmatic/refs/heads/main/security/pubmatic-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Advertising
- AdTech
- Programmatic Advertising
- Supply Side Platform
- SSP
- Header Bidding
- OpenWrap
- Prebid
- OpenRTB
- Connected TV
- CTV
- Mobile Advertising
- Commerce Media
- Retail Media
- Identity
- Curation
- Auction Packages
- Agentic AI
---
