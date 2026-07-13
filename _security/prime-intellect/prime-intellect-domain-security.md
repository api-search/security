---
api_specs:
- filename: prime-intellect-compute-api-openapi.yml
  format: yaml
  label: Prime Intellect Compute API
  slug: prime-intellect-compute-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prime-intellect/refs/heads/main/openapi/prime-intellect-compute-api-openapi.yml
- filename: prime-intellect-sandbox-api-openapi.yml
  format: yaml
  label: Prime Intellect Sandbox API
  slug: prime-intellect-sandbox-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prime-intellect/refs/heads/main/openapi/prime-intellect-sandbox-api-openapi.yml
- filename: prime-intellect-training-api-openapi.yml
  format: yaml
  label: Prime Intellect Training API
  slug: prime-intellect-training-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prime-intellect/refs/heads/main/openapi/prime-intellect-training-api-openapi.yml
- filename: prime-intellect-evaluations-api-openapi.yml
  format: yaml
  label: Prime Intellect Evaluations API
  slug: prime-intellect-evaluations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prime-intellect/refs/heads/main/openapi/prime-intellect-evaluations-api-openapi.yml
- filename: prime-intellect-inference-api-openapi.yml
  format: yaml
  label: Prime Intellect Inference API
  slug: prime-intellect-inference-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prime-intellect/refs/heads/main/openapi/prime-intellect-inference-api-openapi.yml
- filename: prime-intellect-platform-api-openapi.yml
  format: yaml
  label: Prime Intellect Platform API
  slug: prime-intellect-platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prime-intellect/refs/heads/main/openapi/prime-intellect-platform-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: primeintellect.ai
  spf: true
hosts:
- cert_expires: Oct  2 05:20:38 2026 GMT
  host: www.primeintellect.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  2 17:32:32 2026 GMT
  host: app.primeintellect.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 25 05:48:34 2026 GMT
  host: docs.primeintellect.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Prime Intellect Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Prime Intellect, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Prime Intellect
provider_slug: prime-intellect
slug: prime-intellect-domain-security
source_filename: prime-intellect-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.primeintellect.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 05:20:38 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: app.primeintellect.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  2 17:32:32 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.primeintellect.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 05:48:34 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: primeintellect.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/prime-intellect/refs/heads/main/security/prime-intellect-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- AI
- Artificial Intelligence
- Reinforcement Learning
- GPU Compute
- Decentralized Compute
- Foundation Models
- Inference
- Sandboxes
- Training
- Environments
- Evaluations
- LoRA
- Open Source
- Agents
---
