---
api_specs:
- filename: armada-orchestrator-openapi-original.yml
  format: yaml
  label: Armada Bridge Orchestrator API
  slug: armada-bridge-orchestrator-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/armada/refs/heads/main/openapi/armada-orchestrator-openapi-original.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: armada.ai
  spf: true
hosts:
- cert_expires: Oct 14 07:24:53 2026 GMT
  host: armada.ai
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Armada Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Armada, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Armada
provider_slug: armada
slug: armada-domain-security
source_filename: armada-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: armada.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 14 07:24:53 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\ndomains:\n- domain: armada.ai\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/armada/refs/heads/main/security/armada-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Edge Computing
- GPU Cloud
- Infrastructure
- Artificial Intelligence
- Kubernetes
- Bare Metal
- IoT
- Orchestration
- Sovereign Cloud
---
