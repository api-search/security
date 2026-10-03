---
api_specs:
- filename: aureliusagent-dev-ai-generation-api-openapi.yml
  format: yaml
  label: WunderCorp AI Generation API
  slug: aureliusagent-dev-ai-generation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aureliusagent-dev/refs/heads/main/openapi/aureliusagent-dev-ai-generation-api-openapi.yml
- filename: aureliusagent-dev-app-planning-api-openapi.yml
  format: yaml
  label: WunderCorp App Planning API
  slug: aureliusagent-dev-app-planning-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aureliusagent-dev/refs/heads/main/openapi/aureliusagent-dev-app-planning-api-openapi.yml
- filename: aureliusagent-dev-builderstudio-api-openapi.yml
  format: yaml
  label: WunderCorp Builder Studio API
  slug: aureliusagent-dev-builderstudio-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aureliusagent-dev/refs/heads/main/openapi/aureliusagent-dev-builderstudio-api-openapi.yml
- filename: aureliusagent-dev-capacity-api-openapi.yml
  format: yaml
  label: WunderCorp Capacity API
  slug: aureliusagent-dev-capacity-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aureliusagent-dev/refs/heads/main/openapi/aureliusagent-dev-capacity-api-openapi.yml
- filename: aureliusagent-dev-commerce-api-openapi.yml
  format: yaml
  label: WunderCorp Commerce API
  slug: aureliusagent-dev-commerce-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aureliusagent-dev/refs/heads/main/openapi/aureliusagent-dev-commerce-api-openapi.yml
- filename: aureliusagent-dev-inference-gateway-api-openapi.yml
  format: yaml
  label: WunderCorp Inference Gateway API
  slug: aureliusagent-dev-inference-gateway-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aureliusagent-dev/refs/heads/main/openapi/aureliusagent-dev-inference-gateway-api-openapi.yml
- filename: aureliusagent-dev-machine-payments-api-openapi.yml
  format: yaml
  label: WunderCorp Machine Payments API
  slug: aureliusagent-dev-machine-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aureliusagent-dev/refs/heads/main/openapi/aureliusagent-dev-machine-payments-api-openapi.yml
- filename: aureliusagent-dev-mpp-api-openapi.yml
  format: yaml
  label: WunderCorp Mpp API
  slug: aureliusagent-dev-mpp-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aureliusagent-dev/refs/heads/main/openapi/aureliusagent-dev-mpp-api-openapi.yml
- filename: aureliusagent-dev-openmodel-pricing-api-openapi.yml
  format: yaml
  label: WunderCorp OpenModel Pricing API
  slug: aureliusagent-dev-openmodel-pricing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aureliusagent-dev/refs/heads/main/openapi/aureliusagent-dev-openmodel-pricing-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: aureliusagent.dev
  spf: false
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: wundercorp.co
  spf: false
hosts:
- cert_expires: Dec 19 23:59:59 2026 GMT
  host: aureliusagent.dev
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 21 23:59:59 2026 GMT
  host: rpc.aureliusagent.dev
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar 26 23:59:59 2027 GMT
  host: wundercorp.co
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Aureliusagent Dev Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for WunderCorp, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: WunderCorp
provider_slug: aureliusagent-dev
slug: aureliusagent-dev-domain-security
source_filename: aureliusagent-dev-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: aureliusagent.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 19 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: rpc.aureliusagent.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 21 23:59:59 2026 GMT\n  hsts: null\n- host: wundercorp.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 26 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: aureliusagent.dev\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n- domain: wundercorp.co\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aureliusagent-dev/refs/heads/main/security/aureliusagent-dev-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Agents
- A2A
- Machine Payments
- MPP
- HTTP 402
- Artificial Intelligence
- Inference Gateway
- Code Generation
- Developer Tools
- Compute Capacity
- Orchestration
---
