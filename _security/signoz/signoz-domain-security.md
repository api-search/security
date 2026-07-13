---
api_specs:
- filename: signoz-openapi.yml
  format: yaml
  label: SigNoz
  slug: signoz
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/signoz/refs/heads/main/openapi/signoz-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: signoz.io
  spf: true
hosts:
- cert_expires: Sep 13 13:45:54 2026 GMT
  host: signoz.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Signoz Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SigNoz, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: SigNoz
provider_slug: signoz
slug: signoz-domain-security
source_filename: signoz-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: signoz.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 13:45:54 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: signoz.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/signoz/refs/heads/main/security/signoz-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- APM
- Alerting
- Cloud Monitoring
- Dashboards
- Distributed Tracing
- Infrastructure Monitoring
- Logs
- Metrics
- Observability
- OpenTelemetry
- Open Source
---
