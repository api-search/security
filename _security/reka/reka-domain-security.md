---
api_specs:
- filename: reka-chat-api-openapi.yml
  format: yaml
  label: Reka Chat API
  slug: reka-chat-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reka/refs/heads/main/openapi/reka-chat-api-openapi.yml
- filename: reka-clips-api-openapi.yml
  format: yaml
  label: Reka Clips API
  slug: reka-clips-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reka/refs/heads/main/openapi/reka-clips-api-openapi.yml
- filename: reka-models-api-openapi.yml
  format: yaml
  label: Reka Models API
  slug: reka-models-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reka/refs/heads/main/openapi/reka-models-api-openapi.yml
- filename: reka-qa-api-openapi.yml
  format: yaml
  label: Reka QA API
  slug: reka-qa-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reka/refs/heads/main/openapi/reka-qa-api-openapi.yml
- filename: reka-research-api-openapi.yml
  format: yaml
  label: Reka Research API
  slug: reka-research-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reka/refs/heads/main/openapi/reka-research-api-openapi.yml
- filename: reka-search-api-openapi.yml
  format: yaml
  label: Reka Search API
  slug: reka-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reka/refs/heads/main/openapi/reka-search-api-openapi.yml
- filename: reka-speech-api-openapi.yml
  format: yaml
  label: Reka Speech API
  slug: reka-speech-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reka/refs/heads/main/openapi/reka-speech-api-openapi.yml
- filename: reka-videogroups-api-openapi.yml
  format: yaml
  label: Reka VideoGroups API
  slug: reka-videogroups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reka/refs/heads/main/openapi/reka-videogroups-api-openapi.yml
- filename: reka-videos-api-openapi.yml
  format: yaml
  label: Reka Videos API
  slug: reka-videos-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reka/refs/heads/main/openapi/reka-videos-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "ssl.com"
  - 0 issuewild "amazon.com"
  - 0 issuewild "awstrust.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "globalsign.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: reka.ai
  spf: true
hosts:
- cert_expires: Sep 30 15:01:52 2026 GMT
  host: reka.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 20 15:15:03 2026 GMT
  host: docs.reka.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 10 19:37:59 2026 GMT
  host: api.reka.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Reka Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Reka, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Reka
provider_slug: reka
slug: reka-domain-security
source_filename: reka-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: reka.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 15:01:52 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.reka.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 15:15:03 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.reka.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 10 19:37:59 2026 GMT\n  hsts: null\ndomains:\n- domain: reka.ai\n  dnssec: false\n  caa:\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"amazon.com\"\n  - 0 issuewild \"awstrust.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"globalsign.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/reka/refs/heads/main/security/reka-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Artificial Intelligence
- Multimodal
- Large Language Models
- Vision
- Speech
- Foundation Models
- OpenAI-Compatible
- SDK
- Enterprise
- On-Premises
---
