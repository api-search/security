---
api_specs:
- filename: openapi.json
  format: json
  label: DietlyAPI
  slug: dietlyapi
  spec_type: OpenAPI
  url: https://www.getdietly.com/openapi.json
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: getdietly.com
  spf: false
hosts:
- cert_expires: Nov  8 18:46:10 2026 GMT
  host: www.getdietly.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  8 18:46:10 2026 GMT
  host: api.getdietly.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: Dietlyapi Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for DietlyAPI, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: DietlyAPI
provider_slug: dietlyapi
slug: dietlyapi-domain-security
source_filename: dietlyapi-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-03'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.getdietly.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  8 18:46:10 2026 GMT\n  hsts: false\n- host: api.getdietly.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  8 18:46:10 2026 GMT\n  hsts: false\ndomains:\n- domain: getdietly.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dietlyapi/refs/heads/main/security/dietlyapi-domain-security.yml
summary_line: TLSv1.3
tags:
- Food
- Nutrition
- Barcodes
- open-food-facts
- Health
- Open Data
---
