---
api_specs:
- filename: housesigma-blog-content-openapi.yml
  format: yaml
  label: HouseSigma Blog Content API
  slug: housesigma-blog-content-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/housesigma/refs/heads/main/openapi/housesigma-blog-content-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: housesigma.com
  spf: true
hosts:
- cert_expires: Oct  9 03:17:20 2026 GMT
  host: housesigma.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Housesigma Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for HouseSigma, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: HouseSigma
provider_slug: housesigma
slug: housesigma-domain-security
source_filename: housesigma-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: housesigma.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  9 03:17:20 2026 GMT\n  hsts: false\ndomains:\n- domain: housesigma.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/housesigma/refs/heads/main/security/housesigma-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Real-Estate
- Canada
- Property Listings
- MLS
- Valuation
- AVM
- PropTech
- Rentals
- Blog
- Content
- WordPress
- oEmbed
- Ontario
- British Columbia
- Toronto
---
