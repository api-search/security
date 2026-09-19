---
api_specs:
- filename: standard-compute-chat-api-openapi.yml
  format: yaml
  label: Standard Compute Chat API
  slug: standard-compute-chat-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/standard-compute/refs/heads/main/openapi/standard-compute-chat-api-openapi.yml
- filename: standard-compute-completions-api-openapi.yml
  format: yaml
  label: Standard Compute Completions API
  slug: standard-compute-completions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/standard-compute/refs/heads/main/openapi/standard-compute-completions-api-openapi.yml
- filename: standard-compute-healthz-api-openapi.yml
  format: yaml
  label: Standard Compute Healthz API
  slug: standard-compute-healthz-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/standard-compute/refs/heads/main/openapi/standard-compute-healthz-api-openapi.yml
- filename: standard-compute-install-ps1-api-openapi.yml
  format: yaml
  label: Standard Compute Install.ps1 API
  slug: standard-compute-install-ps1-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/standard-compute/refs/heads/main/openapi/standard-compute-install-ps1-api-openapi.yml
- filename: standard-compute-install-sh-api-openapi.yml
  format: yaml
  label: Standard Compute Install.sh API
  slug: standard-compute-install-sh-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/standard-compute/refs/heads/main/openapi/standard-compute-install-sh-api-openapi.yml
- filename: standard-compute-messages-api-openapi.yml
  format: yaml
  label: Standard Compute Messages API
  slug: standard-compute-messages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/standard-compute/refs/heads/main/openapi/standard-compute-messages-api-openapi.yml
- filename: standard-compute-models-api-openapi.yml
  format: yaml
  label: Standard Compute Models API
  slug: standard-compute-models-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/standard-compute/refs/heads/main/openapi/standard-compute-models-api-openapi.yml
- filename: standard-compute-responses-api-openapi.yml
  format: yaml
  label: Standard Compute Responses API
  slug: standard-compute-responses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/standard-compute/refs/heads/main/openapi/standard-compute-responses-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: standardcompute.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: stdcmpt.com
  spf: false
hosts:
- cert_expires: Oct 24 17:51:14 2026 GMT
  host: standardcompute.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 12 16:42:53 2026 GMT
  host: api.stdcmpt.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: Standard Compute Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Standard Compute, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Standard Compute
provider_slug: standard-compute
slug: standard-compute-domain-security
source_filename: standard-compute-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: standardcompute.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 24 17:51:14 2026 GMT\n  hsts: false\n- host: api.stdcmpt.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 12 16:42:53 2026 GMT\n  hsts: null\ndomains:\n- domain: standardcompute.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: stdcmpt.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/standard-compute/refs/heads/main/security/standard-compute-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- LLM API
- Flat Rate
- Subscription
- AI Agents
- Inference
- Model Routing
- AI Gateway
- Developer Tools
- Coding Agents
- OpenAI-Compatible
---
