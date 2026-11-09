---
api_specs:
- filename: agentgates-ai-compute-api-openapi.yml
  format: yaml
  label: Agentgates Compute API
  slug: agentgates-ai-compute-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentgates-ai/openapi/agentgates-ai-compute-api-openapi.yml
- filename: agentgates-ai-directory-api-openapi.yml
  format: yaml
  label: Agentgates Directory API
  slug: agentgates-ai-directory-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentgates-ai/openapi/agentgates-ai-directory-api-openapi.yml
- filename: agentgates-ai-inference-api-openapi.yml
  format: yaml
  label: Agentgates Inference API
  slug: agentgates-ai-inference-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentgates-ai/openapi/agentgates-ai-inference-api-openapi.yml
- filename: agentgates-ai-llms-txt-api-openapi.yml
  format: yaml
  label: Agentgates Llms.txt API
  slug: agentgates-ai-llms-txt-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentgates-ai/openapi/agentgates-ai-llms-txt-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "sectigo.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: agentgates.ai
  spf: true
hosts:
- cert_expires: Dec 11 12:47:20 2026 GMT
  host: agentgates.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Agentgates Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Agentgates, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Agentgates
provider_slug: agentgates-ai
slug: agentgates-ai-domain-security
source_filename: agentgates-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: agentgates.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 11 12:47:20 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: agentgates.ai\n  dnssec: false\n  caa:\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/agentgates-ai/security/agentgates-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Artificial Intelligence
- Compute
- Inference
- Blockchain
- Payments
---
