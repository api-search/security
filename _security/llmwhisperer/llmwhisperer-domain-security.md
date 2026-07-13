---
api_specs:
- filename: llmwhisperer-openapi.yml
  format: yaml
  label: LLMWhisperer Whisper Extraction API
  slug: whisper-extraction-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/llmwhisperer/refs/heads/main/openapi/llmwhisperer-openapi.yml
- filename: llmwhisperer-openapi.yml
  format: yaml
  label: LLMWhisperer Whisper Status API
  slug: whisper-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/llmwhisperer/refs/heads/main/openapi/llmwhisperer-openapi.yml
- filename: llmwhisperer-openapi.yml
  format: yaml
  label: LLMWhisperer Whisper Retrieve API
  slug: whisper-retrieve-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/llmwhisperer/refs/heads/main/openapi/llmwhisperer-openapi.yml
- filename: llmwhisperer-openapi.yml
  format: yaml
  label: LLMWhisperer Highlights API
  slug: highlights-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/llmwhisperer/refs/heads/main/openapi/llmwhisperer-openapi.yml
- filename: llmwhisperer-openapi.yml
  format: yaml
  label: LLMWhisperer Webhooks API
  slug: webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/llmwhisperer/refs/heads/main/openapi/llmwhisperer-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: unstract.com
  spf: true
hosts:
- cert_expires: Aug 28 07:41:51 2026 GMT
  host: unstract.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 21 22:15:44 2026 GMT
  host: docs.unstract.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  4 23:53:13 2026 GMT
  host: llmwhisperer-api.us-central.unstract.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Llmwhisperer Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for LLMWhisperer, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: LLMWhisperer
provider_slug: llmwhisperer
slug: llmwhisperer-domain-security
source_filename: llmwhisperer-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: unstract.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 28 07:41:51 2026 GMT\n  hsts: false\n- host: docs.unstract.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 21 22:15:44 2026 GMT\n  hsts: false\n- host: llmwhisperer-api.us-central.unstract.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 23:53:13 2026 GMT\n  hsts: null\ndomains:\n- domain: unstract.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/llmwhisperer/refs/heads/main/security/llmwhisperer-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- AI
- LLM
- Document Extraction
- OCR
- Text Extraction
---
