---
api_specs:
- filename: devtron-openapi-original.yml
  format: yaml
  label: Devtron Orchestrator API
  slug: devtron-orchestrator-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/devtron/refs/heads/main/openapi/devtron-openapi-original.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: devtron.ai
  spf: true
hosts:
- cert_expires: Oct  2 00:55:56 2026 GMT
  host: devtron.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Devtron Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Devtron, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Devtron
provider_slug: devtron
slug: devtron-domain-security
source_filename: devtron-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: devtron.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 00:55:56 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: devtron.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/devtron/refs/heads/main/security/devtron-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- DevOps
- Kubernetes
- CI/CD
- GitOps
- Platform Engineering
- Software Delivery
- FinOps
- Observability
---
