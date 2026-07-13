---
api_specs:
- filename: trubrics-openapi.yml
  format: yaml
  label: Trubrics Event Ingestion API
  slug: trubrics-event-ingestion-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trubrics/refs/heads/main/openapi/trubrics-openapi.yml
- filename: trubrics-openapi.yml
  format: yaml
  label: Trubrics LLM Event Ingestion API
  slug: trubrics-llm-event-ingestion-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trubrics/refs/heads/main/openapi/trubrics-openapi.yml
- filename: trubrics-openapi.yml
  format: yaml
  label: Trubrics Experiences and Feedback API
  slug: trubrics-experiences-feedback-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trubrics/refs/heads/main/openapi/trubrics-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: trubrics.com
  spf: true
hosts:
- cert_expires: Sep 30 14:00:27 2026 GMT
  host: www.trubrics.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 31 05:29:20 2026 GMT
  host: docs.trubrics.com
  hsts: true
  hsts_max_age: 31556952
  https: true
  tls_version: TLSv1.3
- host: app.trubrics.com
  https: false
kind: domain-security
layout: security
method: probed
name: Trubrics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Trubrics, probed live across 3 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Trubrics
provider_slug: trubrics
slug: trubrics-domain-security
source_filename: trubrics-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.trubrics.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 14:00:27 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.trubrics.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 31 05:29:20 2026 GMT\n  hsts: true\n  hsts_max_age: 31556952\n- host: app.trubrics.com\n  https: false\ndomains:\n- domain: trubrics.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/trubrics/refs/heads/main/security/trubrics-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- AI
- LLM
- Product Analytics
- Event Tracking
- Feedback
---
