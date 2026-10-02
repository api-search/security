---
api_specs:
- filename: postfinder-io-nearby-api-openapi.yml
  format: yaml
  label: Postfinder Nearby API
  slug: postfinder-io-nearby-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/postfinder-io/refs/heads/main/openapi/postfinder-io-nearby-api-openapi.yml
- filename: postfinder-io-places-api-openapi.yml
  format: yaml
  label: Postfinder Places API
  slug: postfinder-io-places-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/postfinder-io/refs/heads/main/openapi/postfinder-io-places-api-openapi.yml
- filename: postfinder-io-postcodes-api-openapi.yml
  format: yaml
  label: Postfinder Postcodes API
  slug: postfinder-io-postcodes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/postfinder-io/refs/heads/main/openapi/postfinder-io-postcodes-api-openapi.yml
- filename: postfinder-io-reference-api-openapi.yml
  format: yaml
  label: Postfinder Reference API
  slug: postfinder-io-reference-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/postfinder-io/refs/heads/main/openapi/postfinder-io-reference-api-openapi.yml
- filename: postfinder-io-search-api-openapi.yml
  format: yaml
  label: Postfinder Search API
  slug: postfinder-io-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/postfinder-io/refs/heads/main/openapi/postfinder-io-search-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: postfinder.io
  spf: true
hosts:
- cert_expires: Dec  7 05:08:06 2026 GMT
  host: postfinder.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Postfinder Io Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Postfinder, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Postfinder
provider_slug: postfinder-io
slug: postfinder-io-domain-security
source_filename: postfinder-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: postfinder.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  7 05:08:06 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: postfinder.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/postfinder-io/refs/heads/main/security/postfinder-io-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Address
- Autocomplete
- Logistics
- Australia
---
