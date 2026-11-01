---
api_specs:
- filename: metal-sentinel-api-openapi.json
  format: json
  label: Metal Sentinel API API
  slug: metal-sentinel-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/metal-sentinel/openapi/_original/metal-sentinel-api-openapi.json
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: metal-sentinel.com
  spf: true
hosts:
- cert_expires: Jan 16 23:34:20 2027 GMT
  host: metal-sentinel.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Metal Sentinel Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Metal Sentinel, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Metal Sentinel
provider_slug: metal-sentinel
slug: metal-sentinel-domain-security
source_filename: metal-sentinel-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-24'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: metal-sentinel.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 16 23:34:20 2027 GMT\n  hsts: false\ndomains:\n- domain: metal-sentinel.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/metal-sentinel/security/metal-sentinel-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Financial Data
- Metals
- API
- Real-time
---
