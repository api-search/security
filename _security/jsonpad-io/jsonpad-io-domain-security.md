---
api_specs:
- filename: jsonpad-io-openapi-generated.yml
  format: yaml
  label: jsonpad-io API
  slug: jsonpad-io-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/jsonpad-io/openapi/_ae-authored/jsonpad-io-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: jsonpad.io
  spf: false
hosts:
- cert_expires: Apr 21 23:59:59 2027 GMT
  host: jsonpad.io
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Jsonpad Io Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for jsonpad-io, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=reject).'
provider_name: jsonpad-io
provider_slug: jsonpad-io
slug: jsonpad-io-domain-security
source_filename: jsonpad-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: jsonpad.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Apr 21 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: jsonpad.io\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/jsonpad-io/security/jsonpad-io-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- JSON Storage
- REST API
- No-Code Backend
- Real-time Updates
- Versioning
---
