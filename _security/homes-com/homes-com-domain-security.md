---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: homes.com
  spf: true
hosts:
- cert_expires: Jan 24 23:59:59 2027 GMT
  host: www.homes.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Homes Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Homes.com, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Homes.com
provider_slug: homes-com
slug: homes-com-domain-security
source_filename: homes-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.homes.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 24 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: homes.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/homes-com/refs/heads/main/security/homes-com-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Real-Estate
- United States
- Property Listings
- MLS
- RESO
- IDX
- Rentals
- PropTech
- Portal
- Marketplaces
- Residential Real Estate
- Real Estate Agents
- Brokers
- Listings Syndication
- CoStar Group
---
