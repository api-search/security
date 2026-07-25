---
api_specs:
- filename: jaeger-dependencies-api-openapi.yml
  format: yaml
  label: Jaeger Dependencies API
  slug: jaeger-dependencies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jaeger/refs/heads/main/openapi/jaeger-dependencies-api-openapi.yml
- filename: jaeger-metrics-api-openapi.yml
  format: yaml
  label: Jaeger Metrics API
  slug: jaeger-metrics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jaeger/refs/heads/main/openapi/jaeger-metrics-api-openapi.yml
- filename: jaeger-services-api-openapi.yml
  format: yaml
  label: Jaeger Services API
  slug: jaeger-services-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jaeger/refs/heads/main/openapi/jaeger-services-api-openapi.yml
- filename: jaeger-traces-api-openapi.yml
  format: yaml
  label: Jaeger Traces API
  slug: jaeger-traces-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jaeger/refs/heads/main/openapi/jaeger-traces-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: jaegertracing.io
  spf: false
hosts:
- cert_expires: Sep 30 06:45:19 2026 GMT
  host: www.jaegertracing.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Jaeger Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Jaeger, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Jaeger
provider_slug: jaeger
slug: jaeger-domain-security
source_filename: jaeger-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.jaegertracing.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 06:45:19 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: jaegertracing.io\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/jaeger/refs/heads/main/security/jaeger-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Distributed Tracing
- Microservices
- Monitoring
- Observability
---
