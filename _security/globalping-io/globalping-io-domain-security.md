---
api_specs:
- filename: globalping-io-limits-api-openapi.yml
  format: yaml
  label: Globalping Limits API
  slug: globalping-io-limits-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/globalping-io/openapi/globalping-io-limits-api-openapi.yml
- filename: globalping-io-measurements-api-openapi.yml
  format: yaml
  label: Globalping Measurements API
  slug: globalping-io-measurements-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/globalping-io/openapi/globalping-io-measurements-api-openapi.yml
- filename: globalping-io-probes-api-openapi.yml
  format: yaml
  label: Globalping Probes API
  slug: globalping-io-probes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/globalping-io/openapi/globalping-io-probes-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: globalping.io
  spf: false
hosts:
- cert_expires: Jan 16 03:43:19 2027 GMT
  host: globalping.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Globalping Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Globalping, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Globalping
provider_slug: globalping-io
slug: globalping-io-domain-security
source_filename: globalping-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-10'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: globalping.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 16 03:43:19 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: globalping.io\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/globalping-io/security/globalping-io-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Networks
- Monitoring
- Open Source
- Free
---
