---
api_specs:
- filename: armadaai-armadaai-api-api-openapi.yml
  format: yaml
  label: Armadaai Armadaai API
  slug: armadaai-armadaai-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/armadaai/refs/heads/main/openapi/armadaai-armadaai-api-api-openapi.yml
- filename: armadaai-health-api-openapi.yml
  format: yaml
  label: Armadaai Health API
  slug: armadaai-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/armadaai/refs/heads/main/openapi/armadaai-health-api-openapi.yml
- filename: armadaai-kubernetes-sigs-api-openapi.yml
  format: yaml
  label: Armadaai Kubernetes Sigs API
  slug: armadaai-kubernetes-sigs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/armadaai/refs/heads/main/openapi/armadaai-kubernetes-sigs-api-openapi.yml
- filename: armadaai-metrics-api-openapi.yml
  format: yaml
  label: Armadaai Metrics API
  slug: armadaai-metrics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/armadaai/refs/heads/main/openapi/armadaai-metrics-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: armada.ai
  spf: true
hosts:
- cert_expires: Nov  6 22:14:51 2026 GMT
  host: www.armada.ai
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Armadaai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Armadaai, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Armadaai
provider_slug: armadaai
slug: armadaai-domain-security
source_filename: armadaai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.armada.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  6 22:14:51 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\ndomains:\n- domain: armada.ai\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/armadaai/refs/heads/main/security/armadaai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Edge Computing
- AI Infrastructure
- Hardware
- Software
- Industries
---
