---
api_specs:
- filename: parseable-api-openapi-generated.yml
  format: yaml
  label: Parseable API Reference API
  slug: api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/parseable/openapi/_ae-authored/parseable-api-openapi-generated.yml
- filename: parseable-core-openapi-generated.yml
  format: yaml
  label: Parseable core API
  slug: core-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/parseable/openapi/_ae-authored/parseable-core-openapi-generated.yml
- filename: parseable-ingest-data-openapi-generated.yml
  format: yaml
  label: Parseable ingest data API
  slug: ingest-data-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/parseable/openapi/_ae-authored/parseable-ingest-data-openapi-generated.yml
- filename: parseable-user-guide-openapi-generated.yml
  format: yaml
  label: Parseable user guide API
  slug: user-guide-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/parseable/openapi/_ae-authored/parseable-user-guide-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: parseable.com
  spf: true
hosts:
- cert_expires: Dec 23 12:31:37 2026 GMT
  host: parseable.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Parseable Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Parseable, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Parseable
provider_slug: parseable
slug: parseable-domain-security
source_filename: parseable-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-15'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: parseable.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 23 12:31:37 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: parseable.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/parseable/security/parseable-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Observability
- OpenTelemetry
- Rust
- Cloud
- Data Lake
- Company
---
