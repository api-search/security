---
api_specs:
- filename: hamming-ai-datasets-api-openapi.yml
  format: yaml
  label: Hamming AI Datasets API
  slug: hamming-ai-datasets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hamming-ai/refs/heads/main/openapi/hamming-ai-datasets-api-openapi.yml
- filename: hamming-ai-experiments-api-openapi.yml
  format: yaml
  label: Hamming AI Experiments API
  slug: hamming-ai-experiments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hamming-ai/refs/heads/main/openapi/hamming-ai-experiments-api-openapi.yml
- filename: hamming-ai-monitoring-api-openapi.yml
  format: yaml
  label: Hamming AI Monitoring API
  slug: hamming-ai-monitoring-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hamming-ai/refs/heads/main/openapi/hamming-ai-monitoring-api-openapi.yml
- filename: hamming-ai-prompts-api-openapi.yml
  format: yaml
  label: Hamming AI Prompts API
  slug: hamming-ai-prompts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hamming-ai/refs/heads/main/openapi/hamming-ai-prompts-api-openapi.yml
- filename: hamming-ai-scoring-api-openapi.yml
  format: yaml
  label: Hamming AI Scoring API
  slug: hamming-ai-scoring-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hamming-ai/refs/heads/main/openapi/hamming-ai-scoring-api-openapi.yml
- filename: hamming-ai-voice-testing-api-openapi.yml
  format: yaml
  label: Hamming AI Voice Testing API
  slug: hamming-ai-voice-testing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hamming-ai/refs/heads/main/openapi/hamming-ai-voice-testing-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "ssl.com"
  - 0 iodef "mailto:sumanyu@hamming.ai"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: hamming.ai
  spf: true
hosts:
- cert_expires: Oct  6 13:37:04 2026 GMT
  host: hamming.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 13 04:31:48 2026 GMT
  host: docs.hamming.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 13 04:31:48 2026 GMT
  host: app.hamming.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Hamming Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Hamming AI, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Hamming AI
provider_slug: hamming-ai
slug: hamming-ai-domain-security
source_filename: hamming-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: hamming.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 13:37:04 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.hamming.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 04:31:48 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: app.hamming.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 04:31:48 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: hamming.ai\n  dnssec: true\n  caa:\n  - 0 issuewild \"ssl.com\"\n  - 0 iodef \"mailto:sumanyu@hamming.ai\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hamming-ai/refs/heads/main/security/hamming-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- AI
- Voice Agents
- LLM
- Testing
- Evaluation
- Observability
---
