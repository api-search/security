---
api_specs:
- filename: litellm-openapi.yml
  format: yaml
  label: LiteLLM Chat Completions API
  slug: chat-completions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/litellm/refs/heads/main/openapi/litellm-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: litellm.ai
  spf: true
hosts:
- cert_expires: Sep 12 18:35:09 2026 GMT
  host: www.litellm.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 13 19:15:58 2026 GMT
  host: docs.litellm.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Litellm Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for LiteLLM, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: LiteLLM
provider_slug: litellm
slug: litellm-domain-security
source_filename: litellm-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.litellm.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 12 18:35:09 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.litellm.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 13 19:15:58 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: litellm.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/litellm/refs/heads/main/security/litellm-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Gateways
---
