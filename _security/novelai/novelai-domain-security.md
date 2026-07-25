---
api_specs:
- filename: novelai-ai-api-openapi.yml
  format: yaml
  label: NovelAI /ai/ API
  slug: novelai-ai-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/novelai/refs/heads/main/openapi/novelai-ai-api-openapi.yml
- filename: novelai-ai-module-api-openapi.yml
  format: yaml
  label: NovelAI /ai/module/ API
  slug: novelai-ai-module-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/novelai/refs/heads/main/openapi/novelai-ai-module-api-openapi.yml
- filename: novelai-default-api-openapi.yml
  format: yaml
  label: NovelAI / API
  slug: novelai-default-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/novelai/refs/heads/main/openapi/novelai-default-api-openapi.yml
- filename: novelai-user-api-openapi.yml
  format: yaml
  label: NovelAI /user/ API
  slug: novelai-user-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/novelai/refs/heads/main/openapi/novelai-user-api-openapi.yml
- filename: novelai-user-subscription-api-openapi.yml
  format: yaml
  label: NovelAI /user/subscription/ API
  slug: novelai-user-subscription-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/novelai/refs/heads/main/openapi/novelai-user-subscription-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  dmarc: false
  dnssec: false
  domain: novelai.net
  spf: true
hosts:
- cert_expires: Sep 19 21:57:19 2026 GMT
  host: novelai.net
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  5 18:46:54 2026 GMT
  host: api.novelai.net
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Novelai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for NovelAI, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: NovelAI
provider_slug: novelai
slug: novelai-domain-security
source_filename: novelai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: novelai.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 19 21:57:19 2026 GMT\n  hsts: false\n- host: api.novelai.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 18:46:54 2026 GMT\n  hsts: false\ndomains:\n- domain: novelai.net\n  dnssec: false\n  caa:\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/novelai/refs/heads/main/security/novelai-domain-security.yml
summary_line: TLSv1.3
tags:
- AI
- Image Generation
- LLM
- Storytelling
---
