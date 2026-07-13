---
api_specs:
- filename: fluent-bit-monitoring-openapi.yml
  format: yaml
  label: Fluent Bit Monitoring HTTP API
  slug: fluent-bit-monitoring-http-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fluent-bit/refs/heads/main/openapi/fluent-bit-monitoring-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: fluentbit.io
  spf: false
hosts:
- cert_expires: Aug 27 01:24:15 2026 GMT
  host: fluentbit.io
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  1 01:19:23 2026 GMT
  host: docs.fluentbit.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- host: 127.0.0.1
  https: false
kind: domain-security
layout: security
method: probed
name: Fluent Bit Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Fluent Bit, probed live across 3 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Fluent Bit
provider_slug: fluent-bit
slug: fluent-bit-domain-security
source_filename: fluent-bit-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: fluentbit.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 27 01:24:15 2026 GMT\n  hsts: false\n- host: docs.fluentbit.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  1 01:19:23 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: 127.0.0.1\n  https: false\ndomains:\n- domain: fluentbit.io\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fluent-bit/refs/heads/main/security/fluent-bit-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Logging
- Observability
- Metrics
- Open Source
---
