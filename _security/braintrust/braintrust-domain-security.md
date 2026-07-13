---
api_specs:
- filename: braintrust-openapi.json
  format: json
  label: Braintrust API
  slug: braintrust-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/braintrust/refs/heads/main/openapi/braintrust-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: braintrust.dev
  spf: true
hosts:
- cert_expires: Sep 22 20:45:31 2026 GMT
  host: www.braintrust.dev
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  7 23:59:59 2026 GMT
  host: api.braintrust.dev
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Braintrust Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Braintrust, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Braintrust
provider_slug: braintrust
slug: braintrust-domain-security
source_filename: braintrust-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.braintrust.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 22 20:45:31 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.braintrust.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  7 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: braintrust.dev\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/braintrust/refs/heads/main/security/braintrust-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Artificial Intelligence
- LLM
- Observability
- Evaluation
- Experiments
- Datasets
- Prompts
- Tracing
- Monitoring
- Scoring
- AI Engineering
- Generative AI
---
