---
api_specs:
- filename: dat-freight-openapi.yml
  format: yaml
  label: DAT Identity & Token API
  slug: dat-freight-identity-token-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dat-freight/refs/heads/main/openapi/dat-freight-openapi.yml
- filename: dat-freight-openapi.yml
  format: yaml
  label: DAT Load Board Search API
  slug: dat-freight-load-board-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dat-freight/refs/heads/main/openapi/dat-freight-openapi.yml
- filename: dat-freight-openapi.yml
  format: yaml
  label: DAT Freight Posting API
  slug: dat-freight-posting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dat-freight/refs/heads/main/openapi/dat-freight-openapi.yml
- filename: dat-freight-openapi.yml
  format: yaml
  label: DAT RateView Rate Lookup API
  slug: dat-freight-rateview-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dat-freight/refs/heads/main/openapi/dat-freight-openapi.yml
- filename: dat-freight-openapi.yml
  format: yaml
  label: DAT BookNow API
  slug: dat-freight-booknow-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dat-freight/refs/heads/main/openapi/dat-freight-openapi.yml
- filename: dat-freight-openapi.yml
  format: yaml
  label: DAT Tracking API
  slug: dat-freight-tracking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dat-freight/refs/heads/main/openapi/dat-freight-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: dat.com
  spf: true
hosts:
- cert_expires: Sep 17 16:01:46 2026 GMT
  host: www.dat.com
  hsts: true
  hsts_max_age: 300
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 17 10:07:55 2026 GMT
  host: developer.dat.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 30 23:55:59 2026 GMT
  host: identity.api.dat.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Dat Freight Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for DAT Freight & Analytics, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: DAT Freight & Analytics
provider_slug: dat-freight
slug: dat-freight-domain-security
source_filename: dat-freight-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.dat.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 17 16:01:46 2026 GMT\n  hsts: true\n  hsts_max_age: 300\n- host: developer.dat.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 17 10:07:55 2026 GMT\n  hsts: null\n- host: identity.api.dat.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 23:55:59 2026 GMT\n  hsts: null\ndomains:\n- domain: dat.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dat-freight/refs/heads/main/security/dat-freight-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Freight
- Trucking
- Load Board
- Logistics
- Freight Rates
- RateView
- Supply Chain
- Transportation
- Analytics
---
