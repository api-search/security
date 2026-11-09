---
api_specs:
- filename: feason-com-context-api-openapi.yml
  format: yaml
  label: Feason Context API
  slug: feason-com-context-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/feason-com/openapi/feason-com-context-api-openapi.yml
- filename: feason-com-proof-api-openapi.yml
  format: yaml
  label: Feason Proof API
  slug: feason-com-proof-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/feason-com/openapi/feason-com-proof-api-openapi.yml
- filename: feason-com-well-known-api-openapi.yml
  format: yaml
  label: Feason .well Known API
  slug: feason-com-well-known-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/feason-com/openapi/feason-com-well-known-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: feason.com
  spf: true
hosts:
- cert_expires: Dec 24 10:14:02 2026 GMT
  host: feason.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Feason Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Feason, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Feason
provider_slug: feason-com
slug: feason-com-domain-security
source_filename: feason-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-07'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: feason.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 24 10:14:02 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: feason.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/feason-com/security/feason-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Scripture
- Courses
- Christian History
- Fellowship
- Prayer
---
