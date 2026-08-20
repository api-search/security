---
api_specs:
- filename: rightmove-commercial-listings-openapi.yml
  format: yaml
  label: Rightmove Commercial Listings API
  slug: rightmove-commercial-listings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rightmove/refs/heads/main/openapi/rightmove-commercial-listings-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: rightmove.co.uk
  spf: true
hosts:
- cert_expires: Aug 21 13:53:21 2026 GMT
  host: www.rightmove.co.uk
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 23 15:52:53 2026 GMT
  host: api-docs.rightmove.co.uk
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 21 13:58:51 2026 GMT
  host: api-services.rightmove.co.uk
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Rightmove Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Rightmove, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Rightmove
provider_slug: rightmove
slug: rightmove-domain-security
source_filename: rightmove-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.rightmove.co.uk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 21 13:53:21 2026 GMT\n  hsts: false\n- host: api-docs.rightmove.co.uk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 23 15:52:53 2026 GMT\n  hsts: null\n- host: api-services.rightmove.co.uk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 21 13:58:51 2026 GMT\n  hsts: null\ndomains:\n- domain: rightmove.co.uk\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rightmove/refs/heads/main/security/rightmove-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Real-Estate
- United Kingdom
- Property Listings
- Property Portal
- PropTech
- Rentals
- Commercial Real Estate
- Data Feed
---
