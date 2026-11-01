---
api_specs:
- filename: netalertx-netalertx-api-api-openapi.yml
  format: yaml
  label: NetAlertX API
  slug: netalertx-api-2
  spec_type: OpenAPI
  url: https://artifacts.apis.io/netalertx/openapi/netalertx-netalertx-api-api-openapi.yml
- filename: netalertx-openapi-generated.yml
  format: yaml
  label: NetAlertX API
  slug: netalertx-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/netalertx/openapi/_ae-authored/netalertx-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: netalertx.com
  spf: true
hosts:
- cert_expires: Jan  7 05:41:51 2027 GMT
  host: netalertx.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Netalertx Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for NetAlertX, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: NetAlertX
provider_slug: netalertx
slug: netalertx-domain-security
source_filename: netalertx-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: netalertx.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  7 05:41:51 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: netalertx.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/netalertx/security/netalertx-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Network Monitoring
- Asset Discovery
- Home Automation
- Open Source
- Self-Hosted
---
