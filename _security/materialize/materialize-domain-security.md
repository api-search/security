---
api_specs:
- filename: materialize-openapi.yml
  format: yaml
  label: Materialize HTTP API
  slug: materialize-http-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/materialize/refs/heads/main/openapi/materialize-openapi.yml
- filename: materialize-asyncapi.yml
  format: yaml
  label: Materialize Streaming Sources and Sinks (AsyncAPI)
  slug: materialize-streaming-asyncapi
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/materialize/refs/heads/main/asyncapi/materialize-asyncapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: materialize.com
  spf: true
hosts:
- cert_expires: Oct 16 23:59:59 2026 GMT
  host: materialize.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Materialize Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Materialize, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Materialize
provider_slug: materialize
slug: materialize-domain-security
source_filename: materialize-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: materialize.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 16 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: materialize.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/materialize/refs/heads/main/security/materialize-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Streaming
- Data Warehouse
- SQL
- Real-Time
- PostgreSQL Compatible
---
