---
api_specs:
- filename: openapi.yaml
  format: yaml
  label: Ollama API
  slug: ollama-api
  spec_type: OpenAPI
  url: https://docs.ollama.com/openapi.yaml
- filename: ollama-openai-compatibility-api-openapi.yml
  format: yaml
  label: Ollama OpenAI Compatibility API
  slug: ollama-openai-compatibility-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ollama/refs/heads/main/openapi/ollama-openai-compatibility-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: ollama.com
  spf: true
hosts:
- cert_expires: Sep 18 23:37:57 2026 GMT
  host: ollama.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 20 23:58:29 2026 GMT
  host: docs.ollama.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ollama Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ollama, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Ollama
provider_slug: ollama
slug: ollama-domain-security
source_filename: ollama-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ollama.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 18 23:37:57 2026 GMT\n  hsts: false\n- host: docs.ollama.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 20 23:58:29 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: ollama.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ollama/refs/heads/main/security/ollama-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Artificial Intelligence
- Large Language Models
- Models
---
