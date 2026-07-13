---
api_specs:
- filename: uptrace-openapi.yml
  format: yaml
  label: Uptrace API
  slug: uptrace
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uptrace/refs/heads/main/openapi/uptrace-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: uptrace.dev
  spf: true
hosts:
- cert_expires: Dec 24 23:59:59 2026 GMT
  host: uptrace.dev
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  4 16:43:59 2026 GMT
  host: api.uptrace.dev
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Uptrace Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Uptrace, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Uptrace
provider_slug: uptrace
slug: uptrace-domain-security
source_filename: uptrace-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: uptrace.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 24 23:59:59 2026 GMT\n  hsts: false\n- host: api.uptrace.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  4 16:43:59 2026 GMT\n  hsts: null\ndomains:\n- domain: uptrace.dev\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/uptrace/refs/heads/main/security/uptrace-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- APM
- Observability
- OpenTelemetry
- Distributed Tracing
- Monitoring
---
