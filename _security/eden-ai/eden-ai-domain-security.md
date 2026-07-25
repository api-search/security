---
api_specs:
- filename: eden-ai-audio-api-openapi.yml
  format: yaml
  label: Eden AI Audio API
  slug: eden-ai-audio-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eden-ai/refs/heads/main/openapi/eden-ai-audio-api-openapi.yml
- filename: eden-ai-image-api-openapi.yml
  format: yaml
  label: Eden AI Image API
  slug: eden-ai-image-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eden-ai/refs/heads/main/openapi/eden-ai-image-api-openapi.yml
- filename: eden-ai-ocr-api-openapi.yml
  format: yaml
  label: Eden AI OCR API
  slug: eden-ai-ocr-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eden-ai/refs/heads/main/openapi/eden-ai-ocr-api-openapi.yml
- filename: eden-ai-text-api-openapi.yml
  format: yaml
  label: Eden AI Text API
  slug: eden-ai-text-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eden-ai/refs/heads/main/openapi/eden-ai-text-api-openapi.yml
- filename: eden-ai-translation-api-openapi.yml
  format: yaml
  label: Eden AI Translation API
  slug: eden-ai-translation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eden-ai/refs/heads/main/openapi/eden-ai-translation-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  - 0 issuewild "comodoca.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: edenai.co
  spf: true
- caa:
  - 0 issue "amazon.com"
  dmarc: false
  dnssec: false
  domain: edenai.run
  spf: false
hosts:
- cert_expires: Oct  7 08:18:14 2026 GMT
  host: www.edenai.co
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan  4 23:59:59 2027 GMT
  host: api.edenai.run
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Eden Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Eden AI, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Eden AI
provider_slug: eden-ai
slug: eden-ai-domain-security
source_filename: eden-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.edenai.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 08:18:14 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.edenai.run\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  4 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: edenai.co\n  dnssec: false\n  caa:\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: edenai.run\n  dnssec: false\n  caa:\n  - 0 issue \"amazon.com\"\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/eden-ai/refs/heads/main/security/eden-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Artificial Intelligence
- Emotion
- Emotion Detection
---
