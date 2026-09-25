---
api_specs:
- filename: agenthealthmonitor-xyz-openapi.yml
  format: yaml
  label: Agent Health Monitor API
  slug: agent-health-monitor-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agenthealthmonitor-xyz/refs/heads/main/openapi/agenthealthmonitor-xyz-openapi.yml
- filename: agenthealthmonitor-xyz-verify-openapi.yml
  format: yaml
  label: AHM Verify API
  slug: ahm-verify-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agenthealthmonitor-xyz/refs/heads/main/openapi/agenthealthmonitor-xyz-verify-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: agenthealthmonitor.xyz
  spf: true
hosts:
- cert_expires: Nov 20 12:38:27 2026 GMT
  host: agenthealthmonitor.xyz
  hsts: false
  https: true
  tls_version: TLSv1.2
- cert_expires: Nov 20 12:38:27 2026 GMT
  host: docs.agenthealthmonitor.xyz
  hsts: false
  https: true
  tls_version: TLSv1.2
- cert_expires: Nov 20 12:38:27 2026 GMT
  host: verify.agenthealthmonitor.xyz
  hsts: null
  https: true
  tls_version: TLSv1.2
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Agenthealthmonitor Xyz Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Agent Health Monitor, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Agent Health Monitor
provider_slug: agenthealthmonitor-xyz
slug: agenthealthmonitor-xyz-domain-security
source_filename: agenthealthmonitor-xyz-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: agenthealthmonitor.xyz\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov 20 12:38:27 2026 GMT\n  hsts: false\n- host: docs.agenthealthmonitor.xyz\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov 20 12:38:27 2026 GMT\n  hsts: false\n- host: verify.agenthealthmonitor.xyz\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov 20 12:38:27 2026 GMT\n  hsts: null\ndomains:\n- domain: agenthealthmonitor.xyz\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/agenthealthmonitor-xyz/refs/heads/main/security/agenthealthmonitor-xyz-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- Agents
- Agent Trust
- Risk Scoring
- Wallet Intelligence
- Blockchain
- Base
- x402
- Agentic Commerce
- Monitoring
- Webhook
- Web3
- Verifiable Credentials
- Developer Tools
- Agent-Native
- A2A
---
