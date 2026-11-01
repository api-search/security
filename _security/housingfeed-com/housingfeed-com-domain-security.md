---
api_specs:
- filename: housingfeed-com-sample-api-openapi.yml
  format: yaml
  label: housingfeed-com Sample API
  slug: housingfeed-com-sample-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/housingfeed-com/openapi/housingfeed-com-sample-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: housingfeed.com
  spf: true
hosts:
- cert_expires: Dec  1 14:21:38 2026 GMT
  host: housingfeed.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Housingfeed Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for housingfeed-com, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: housingfeed-com
provider_slug: housingfeed-com
slug: housingfeed-com-domain-security
source_filename: housingfeed-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: housingfeed.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  1 14:21:38 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: housingfeed.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/housingfeed-com/security/housingfeed-com-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- RealEstate
- Rentals
- DataAPI
- US
- Listings
---
