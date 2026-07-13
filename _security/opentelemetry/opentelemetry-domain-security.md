---
api_specs:
- filename: openapi.yml
  format: yaml
  label: OpenTelemetry Protocol (OTLP) HTTP API
  slug: opentelemetry-protocol-otlp-http-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opentelemetry/refs/heads/main/openapi.yml
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org;accounturi=https://acme-v02.api.letsencrypt.org/acme/acct/54403714"
  - 0 issue "letsencrypt.org;accounturi=https://acme-v02.api.letsencrypt.org/acme/acct/2185112545"
  - 0 issue "pki.goog"
  dmarc: false
  dnssec: false
  domain: opentelemetry.io
  spf: false
hosts:
- cert_expires: Oct  1 18:28:58 2026 GMT
  host: opentelemetry.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Opentelemetry Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for OpenTelemetry, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: OpenTelemetry
provider_slug: opentelemetry
slug: opentelemetry-domain-security
source_filename: opentelemetry-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: opentelemetry.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 18:28:58 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: opentelemetry.io\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org;accounturi=https://acme-v02.api.letsencrypt.org/acme/acct/54403714\"\n  - 0 issue \"letsencrypt.org;accounturi=https://acme-v02.api.letsencrypt.org/acme/acct/2185112545\"\n  - 0 issue \"pki.goog\"\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/opentelemetry/refs/heads/main/security/opentelemetry-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Cloud Native
- Logging
- Metrics
- Monitoring
- Observability
- Open Source
- Tracing
---
