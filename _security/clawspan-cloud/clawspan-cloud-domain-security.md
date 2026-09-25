---
api_specs:
- filename: clawspan-cloud-shardlink-control-plane-openapi.yml
  format: yaml
  label: ShardLink Control Plane API
  slug: shardlink-control-plane-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clawspan-cloud/refs/heads/main/openapi/clawspan-cloud-shardlink-control-plane-openapi.yml
- filename: clawspan-cloud-signalhub-gateway-openapi.yml
  format: yaml
  label: SignalHub Gateway API
  slug: signalhub-gateway-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clawspan-cloud/refs/heads/main/openapi/clawspan-cloud-signalhub-gateway-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: clawspan.cloud
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: clawspan.dev
  spf: false
hosts:
- cert_expires: Nov  7 12:45:07 2026 GMT
  host: clawspan.cloud
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 31 10:12:01 2026 GMT
  host: app.clawspan.cloud
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 26 01:46:09 2026 GMT
  host: signalhub.clawspan.dev
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Clawspan Cloud Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ClawSpan, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: ClawSpan
provider_slug: clawspan-cloud
slug: clawspan-cloud-domain-security
source_filename: clawspan-cloud-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: clawspan.cloud\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  7 12:45:07 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: app.clawspan.cloud\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 31 10:12:01 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: signalhub.clawspan.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 26 01:46:09 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: clawspan.cloud\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: clawspan.dev\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/clawspan-cloud/refs/heads/main/security/clawspan-cloud-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- AI Agents
- Agent Marketplace
- Agent-Native
- MCP
- A2A
- Task Orchestration
- Wallet Authentication
- x402
- Marketplace
- Billing
---
