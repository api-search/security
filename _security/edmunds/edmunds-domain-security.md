---
api_specs:
- filename: edmunds-openapi.yml
  format: yaml
  label: Edmunds Dealership API
  slug: edmunds
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/edmunds/refs/heads/main/openapi/edmunds-openapi.yml
- filename: edmunds-openapi.yml
  format: yaml
  label: Edmunds API
  slug: edmunds
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/edmunds/refs/heads/main/openapi/edmunds-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: edmunds.com
  spf: true
hosts:
- cert_expires: Nov 29 23:59:59 2026 GMT
  host: developer.edmunds.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar 10 23:59:59 2027 GMT
  host: api.edmunds.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Edmunds Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Edmunds, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Edmunds
provider_slug: edmunds
slug: edmunds-domain-security
source_filename: edmunds-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developer.edmunds.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 29 23:59:59 2026 GMT\n  hsts: false\n- host: api.edmunds.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 10 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: edmunds.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/edmunds/refs/heads/main/security/edmunds-domain-security.yml
summary_line: TLSv1.3
tags:
- Automobiles
- Cars
- Vehicles
---
