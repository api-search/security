---
api_specs:
- filename: dog-api.yml
  format: yaml
  label: Dog API
  slug: dog-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dog-api/refs/heads/main/openapi/dog-api.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: dog.ceo
  spf: false
hosts:
- cert_expires: Sep  6 23:14:51 2026 GMT
  host: dog.ceo
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Dog Api Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Dog API, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Dog API
provider_slug: dog-api
slug: dog-api-domain-security
source_filename: dog-api-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: dog.ceo\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  6 23:14:51 2026 GMT\n  hsts: false\ndomains:\n- domain: dog.ceo\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dog-api/refs/heads/main/security/dog-api-domain-security.yml
summary_line: TLSv1.3
tags:
- Dogs
- Images
- Open Data
- Open Source
---
