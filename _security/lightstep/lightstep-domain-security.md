---
api_specs:
- filename: openapi
  format: yaml
  label: Lightstep API
  slug: lightstep-api
  spec_type: OpenAPI
  url: https://docs.lightstep.com/openapi
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: lightstep.com
  spf: true
hosts:
- cert_expires: Nov 11 23:59:59 2026 GMT
  host: lightstep.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  8 04:18:01 2026 GMT
  host: docs.lightstep.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Lightstep Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Lightstep, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Lightstep
provider_slug: lightstep
slug: lightstep-domain-security
source_filename: lightstep-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: lightstep.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 11 23:59:59 2026 GMT\n  hsts: null\n- host: docs.lightstep.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  8 04:18:01 2026 GMT\n  hsts: false\ndomains:\n- domain: lightstep.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lightstep/refs/heads/main/security/lightstep-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- APM
- Distributed Tracing
- Microservices
- Monitoring
- Observability
- OpenTelemetry
---
