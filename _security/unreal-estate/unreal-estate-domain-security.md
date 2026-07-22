---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: unrealestate.com
  spf: true
hosts:
- cert_expires: Sep 18 21:18:41 2026 GMT
  host: unrealestate.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Unreal Estate Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Unreal Estate, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Unreal Estate
provider_slug: unreal-estate
slug: unreal-estate-domain-security
source_filename: unreal-estate-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: unrealestate.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 18 21:18:41 2026 GMT\n  hsts: null\ndomains:\n- domain: unrealestate.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/unreal-estate/refs/heads/main/security/unreal-estate-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Real Estate
- PropTech
- MLS
- Flat Fee Listings
- Home Buying
- Home Selling
- Brokerage
- Rentals
---
