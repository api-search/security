---
api_specs:
- filename: raute-io-drivers-api-openapi.yml
  format: yaml
  label: raute-io Drivers API
  slug: raute-io-drivers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/raute-io/openapi/raute-io-drivers-api-openapi.yml
- filename: raute-io-orders-api-openapi.yml
  format: yaml
  label: raute-io Orders API
  slug: raute-io-orders-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/raute-io/openapi/raute-io-orders-api-openapi.yml
- filename: raute-io-tracking-api-openapi.yml
  format: yaml
  label: raute-io Tracking API
  slug: raute-io-tracking-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/raute-io/openapi/raute-io-tracking-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: raute.io
  spf: true
hosts:
- cert_expires: Dec 24 21:49:56 2026 GMT
  host: raute.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Raute Io Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for raute-io, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: raute-io
provider_slug: raute-io
slug: raute-io-domain-security
source_filename: raute-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: raute.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 24 21:49:56 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: raute.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/raute-io/security/raute-io-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Logistics
- Delivery
- Route Planning
- AI
- Fleet Management
---
