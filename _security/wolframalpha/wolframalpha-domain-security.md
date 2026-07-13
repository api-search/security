---
api_specs:
- filename: wolframalpha-llm-api-openapi.yml
  format: yaml
  label: Wolfram|Alpha LLM API
  slug: llm-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wolframalpha/refs/heads/main/openapi/wolframalpha-llm-api-openapi.yml
- filename: wolframalpha-full-results-api-openapi.yml
  format: yaml
  label: Wolfram|Alpha Full Results API
  slug: full-results-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wolframalpha/refs/heads/main/openapi/wolframalpha-full-results-api-openapi.yml
- filename: wolframalpha-short-answers-api-openapi.yml
  format: yaml
  label: Wolfram|Alpha Short Answers API
  slug: short-answers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wolframalpha/refs/heads/main/openapi/wolframalpha-short-answers-api-openapi.yml
- filename: wolframalpha-simple-api-openapi.yml
  format: yaml
  label: Wolfram|Alpha Simple API
  slug: simple-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wolframalpha/refs/heads/main/openapi/wolframalpha-simple-api-openapi.yml
- filename: wolframalpha-spoken-results-api-openapi.yml
  format: yaml
  label: Wolfram|Alpha Spoken Results API
  slug: spoken-results-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wolframalpha/refs/heads/main/openapi/wolframalpha-spoken-results-api-openapi.yml
- filename: wolframalpha-fast-query-recognizer-api-openapi.yml
  format: yaml
  label: Wolfram|Alpha Fast Query Recognizer API
  slug: fast-query-recognizer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wolframalpha/refs/heads/main/openapi/wolframalpha-fast-query-recognizer-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: wolframalpha.com
  spf: true
hosts:
- cert_expires: Dec  3 16:16:35 2026 GMT
  host: www.wolframalpha.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  3 16:16:35 2026 GMT
  host: products.wolframalpha.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  3 16:16:35 2026 GMT
  host: api.wolframalpha.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Wolframalpha Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Wolfram|Alpha, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Wolfram|Alpha
provider_slug: wolframalpha
slug: wolframalpha-domain-security
source_filename: wolframalpha-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.wolframalpha.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  3 16:16:35 2026 GMT\n  hsts: null\n- host: products.wolframalpha.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  3 16:16:35 2026 GMT\n  hsts: null\n- host: api.wolframalpha.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  3 16:16:35 2026 GMT\n  hsts: null\ndomains:\n- domain: wolframalpha.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wolframalpha/refs/heads/main/security/wolframalpha-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- AI
- Artificial Intelligence
- Computational Knowledge
- Machine Learning
- Natural Language Processing
- Public APIs
- Search
---
