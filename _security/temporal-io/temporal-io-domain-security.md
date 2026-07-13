---
api_specs:
- filename: temporal-io-openapi.yml
  format: yaml
  label: Temporal Workflow Service API
  slug: temporal-io-workflow-service-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/temporal-io/refs/heads/main/openapi/temporal-io-openapi.yml
- filename: temporal-io-openapi.yml
  format: yaml
  label: Temporal HTTP API
  slug: temporal-io-http-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/temporal-io/refs/heads/main/openapi/temporal-io-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "amazon.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: temporal.io
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: tmprl.cloud
  spf: true
hosts:
- cert_expires: Sep 21 16:02:20 2026 GMT
  host: temporal.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 27 07:02:20 2026 GMT
  host: docs.temporal.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- host: <namespace>.<account>.tmprl.cloud
  https: false
kind: domain-security
layout: security
method: probed
name: Temporal Io Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Temporal, probed live across 3 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Temporal
provider_slug: temporal-io
slug: temporal-io-domain-security
source_filename: temporal-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: temporal.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 16:02:20 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.temporal.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 27 07:02:20 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: <namespace>.<account>.tmprl.cloud\n  https: false\ndomains:\n- domain: temporal.io\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: tmprl.cloud\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/temporal-io/refs/heads/main/security/temporal-io-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Durable Execution
- Workflow Orchestration
- gRPC
- Workflows
- Open Source
- Temporal Cloud
---
