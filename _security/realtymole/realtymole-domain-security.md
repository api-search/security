---
api_specs:
- filename: realtymole-openapi.yml
  format: yaml
  label: RealtyMole Property Records API
  slug: property-records
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/realtymole/refs/heads/main/openapi/realtymole-openapi.yml
- filename: realtymole-openapi.yml
  format: yaml
  label: RealtyMole Rental Estimate API
  slug: rental-estimate
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/realtymole/refs/heads/main/openapi/realtymole-openapi.yml
- filename: realtymole-openapi.yml
  format: yaml
  label: RealtyMole Sale Estimate API
  slug: sale-estimate
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/realtymole/refs/heads/main/openapi/realtymole-openapi.yml
- filename: realtymole-openapi.yml
  format: yaml
  label: RealtyMole Listings API
  slug: listings
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/realtymole/refs/heads/main/openapi/realtymole-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: realtymole.com
  spf: true
- caa: []
  dmarc: false
  dnssec: true
  domain: rapidapi.com
  spf: true
hosts:
- cert_expires: Dec 18 23:59:59 2026 GMT
  host: www.realtymole.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 18 08:42:50 2026 GMT
  host: rapidapi.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 18 23:59:59 2026 GMT
  host: realty-mole-property-api.p.rapidapi.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Realtymole Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for RealtyMole, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: RealtyMole
provider_slug: realtymole
slug: realtymole-domain-security
source_filename: realtymole-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.realtymole.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 18 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: rapidapi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 18 08:42:50 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: realty-mole-property-api.p.rapidapi.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 18 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: realtymole.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: rapidapi.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/realtymole/refs/heads/main/security/realtymole-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Real Estate
- Property Data
- Rental Estimate
- Valuation
- Listings
---
