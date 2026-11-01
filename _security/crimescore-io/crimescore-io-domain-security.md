---
api_specs:
- filename: crimescore-io-geocode-api-openapi.yml
  format: yaml
  label: crimescore-io Geocode API
  slug: crimescore-io-geocode-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/crimescore-io/openapi/crimescore-io-geocode-api-openapi.yml
- filename: crimescore-io-incidents-api-openapi.yml
  format: yaml
  label: crimescore-io Incidents API
  slug: crimescore-io-incidents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/crimescore-io/openapi/crimescore-io-incidents-api-openapi.yml
- filename: crimescore-io-score-api-openapi.yml
  format: yaml
  label: crimescore-io Score API
  slug: crimescore-io-score-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/crimescore-io/openapi/crimescore-io-score-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: crimescore.io
  spf: true
hosts:
- cert_expires: Apr 12 02:22:58 2027 GMT
  host: crimescore.io
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Crimescore Io Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for crimescore-io, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: crimescore-io
provider_slug: crimescore-io
slug: crimescore-io-domain-security
source_filename: crimescore-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: crimescore.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Apr 12 02:22:58 2027 GMT\n  hsts: false\ndomains:\n- domain: crimescore.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/crimescore-io/security/crimescore-io-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Safety
- RealEstate
- Data
- Mapping
- API
---
