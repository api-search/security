---
api_specs:
- filename: street-co-open-api-openapi.yml
  format: yaml
  label: Street Open API
  slug: street-open-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/street-co/refs/heads/main/openapi/street-co-open-api-openapi.yml
- filename: street-co-property-feed-api-openapi.yml
  format: yaml
  label: Street Property Feed API
  slug: street-property-feed-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/street-co/refs/heads/main/openapi/street-co-property-feed-api-openapi.yml
- filename: street-co-spectre-api-openapi.yml
  format: yaml
  label: Spectre API
  slug: spectre-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/street-co/refs/heads/main/openapi/street-co-spectre-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: street.co.uk
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: uk.com
  spf: true
hosts:
- cert_expires: Dec 27 23:59:59 2026 GMT
  host: street.co.uk
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
- cert_expires: Oct 19 15:49:55 2026 GMT
  host: developers.street.co.uk
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 26 23:59:59 2027 GMT
  host: api.spectre.uk.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Street Co Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Street.co.uk, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Street.co.uk
provider_slug: street-co
slug: street-co-domain-security
source_filename: street-co-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: street.co.uk\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec 27 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developers.street.co.uk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 19 15:49:55 2026 GMT\n  hsts: false\n- host: api.spectre.uk.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 26 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: street.co.uk\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: uk.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/street-co/refs/heads/main/security/street-co-domain-security.yml
summary_line: TLSv1.2 · HSTS · DNSSEC · DMARC
tags:
- Real-Estate
- United Kingdom
- PropTech
- CRM
- Property Listings
- Property Management
- Rentals
- Lettings
- Estate Agency
- Valuation
- Conveyancing
---
