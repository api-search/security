---
api_specs:
- filename: atla-insights-openapi.yaml
  format: yaml
  label: Atla Insights API
  slug: atla-insights-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/atla/refs/heads/main/openapi/atla-insights-openapi.yaml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: atla-ai.com
  spf: true
hosts:
- cert_expires: Oct  7 21:23:22 2026 GMT
  host: www.atla-ai.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- host: app.atla-ai.com
  hsts: null
  https: true
  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: certificate has expired (_ssl.c:1082)'
kind: domain-security
layout: security
method: probed
name: Atla Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Atla, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Atla
provider_slug: atla
slug: atla-domain-security
source_filename: atla-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.atla-ai.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 21:23:22 2026 GMT\n  hsts: null\n- host: app.atla-ai.com\n  https: true\n  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: certificate has\n    expired (_ssl.c:1082)'\n  hsts: null\ndomains:\n- domain: atla-ai.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/atla/refs/heads/main/security/atla-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- SaaS
- Artificial Intelligence
- LLM Evaluation
- AI Agents
- Observability
- Monitoring
- OpenTelemetry
---
