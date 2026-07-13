---
api_specs:
- filename: highlight-otlp-traces-api-openapi.yml
  format: yaml
  label: Highlight OTLP Traces API
  slug: highlight-otlp-traces-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/highlight-io/refs/heads/main/openapi/highlight-otlp-traces-api-openapi.yml
- filename: highlight-otlp-logs-api-openapi.yml
  format: yaml
  label: Highlight OTLP Logs API
  slug: highlight-otlp-logs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/highlight-io/refs/heads/main/openapi/highlight-otlp-logs-api-openapi.yml
- filename: highlight-otlp-metrics-api-openapi.yml
  format: yaml
  label: Highlight OTLP Metrics API
  slug: highlight-otlp-metrics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/highlight-io/refs/heads/main/openapi/highlight-otlp-metrics-api-openapi.yml
- filename: highlight-session-ingestion-api-openapi.yml
  format: yaml
  label: Highlight Session Ingestion API
  slug: highlight-session-ingestion-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/highlight-io/refs/heads/main/openapi/highlight-session-ingestion-api-openapi.yml
- filename: highlight-webhooks-api-openapi.yml
  format: yaml
  label: Highlight Webhooks API
  slug: highlight-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/highlight-io/refs/heads/main/openapi/highlight-webhooks-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: highlight.io
  spf: true
hosts:
- host: www.highlight.io
  hsts: null
  https: true
  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: certificate has expired (_ssl.c:1082)'
- cert_expires: Sep 18 23:59:59 2026 GMT
  host: app.highlight.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 11 23:59:59 2026 GMT
  host: otel.highlight.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Highlight Io Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Highlight (highlight.io), probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Highlight (highlight.io)
provider_slug: highlight-io
slug: highlight-io-domain-security
source_filename: highlight-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.highlight.io\n  https: true\n  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: certificate has\n    expired (_ssl.c:1082)'\n  hsts: null\n- host: app.highlight.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 18 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: otel.highlight.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 11 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: highlight.io\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/highlight-io/refs/heads/main/security/highlight-io-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Observability
- Session Replay
- Error Monitoring
- APM
- Logging
- Tracing
- OpenTelemetry
- Open Source
- Frontend Monitoring
- Full Stack Monitoring
---
