---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: magnite.com
  spf: true
hosts:
- cert_expires: Aug 29 21:26:03 2026 GMT
  host: www.magnite.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Magnite Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Magnite, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Magnite
provider_slug: magnite
slug: magnite-domain-security
source_filename: magnite-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.magnite.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 29 21:26:03 2026 GMT\n  hsts: false\ndomains:\n- domain: magnite.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/magnite/refs/heads/main/security/magnite-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Advertising
- Programmatic Advertising
- Sell-Side Platform
- SSP
- Connected TV
- CTV
- OTT
- Streaming
- Display Advertising
- Video Advertising
- OpenRTB
- Header Bidding
- Ad Tech
- Publisher Monetization
- Demand-Side Integration
---
