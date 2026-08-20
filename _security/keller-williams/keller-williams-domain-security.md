---
api_specs:
- filename: keller-williams-listings-search-openapi.json
  format: json
  label: KW Worldwide Listings Search API
  slug: keller-williams-worldwide-listings-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/keller-williams/refs/heads/main/openapi/keller-williams-listings-search-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: kw.com
  spf: true
hosts:
- cert_expires: Oct 11 04:12:52 2026 GMT
  host: www.kw.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  8 06:57:46 2026 GMT
  host: developer.kw.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 20 23:40:30 2026 GMT
  host: partners.api.kw.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Keller Williams Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Keller Williams, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Keller Williams
provider_slug: keller-williams
slug: keller-williams-domain-security
source_filename: keller-williams-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.kw.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 11 04:12:52 2026 GMT\n  hsts: null\n- host: developer.kw.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  8 06:57:46 2026 GMT\n  hsts: null\n- host: partners.api.kw.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 23:40:30 2026 GMT\n  hsts: null\ndomains:\n- domain: kw.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/keller-williams/refs/heads/main/security/keller-williams-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Real-Estate
- United States
- Residential Real Estate
- Brokerage
- Franchise
- Property Listings
- PropTech
- Agent Platform
- CRM
- Partner APIs
- Marketplace
- Austin Texas
---
