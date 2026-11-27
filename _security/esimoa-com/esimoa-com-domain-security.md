---
api_specs:
- filename: esimoa-com-countries-api-openapi.yml
  format: yaml
  label: esimoa Countries API
  slug: esimoa-com-countries-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/esimoa-com/openapi/esimoa-com-countries-api-openapi.yml
- filename: esimoa-com-esims-api-openapi.yml
  format: yaml
  label: esimoa Esims API
  slug: esimoa-com-esims-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/esimoa-com/openapi/esimoa-com-esims-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: esimoa.com
  spf: true
hosts:
- cert_expires: Feb  2 06:20:41 2027 GMT
  host: esimoa.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: esimoa Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for esimoa, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: esimoa
provider_slug: esimoa-com
slug: esimoa-com-domain-security
source_filename: esimoa-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-07'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: esimoa.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  2 06:20:41 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: esimoa.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/esimoa-com/security/esimoa-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- eSIM
- Travel
- Price Comparison
- Mobile Data
- International
---
