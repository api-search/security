---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: withone.ai
  spf: true
hosts:
- cert_expires: Sep 26 14:04:49 2026 GMT
  host: withone.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 14 13:40:34 2026 GMT
  host: app.withone.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Integration Os Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for IntegrationOS, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: IntegrationOS
provider_slug: integration-os
slug: integration-os-domain-security
source_filename: integration-os-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: withone.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 14:04:49 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: app.withone.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 14 13:40:34 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: withone.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/integration-os/refs/heads/main/security/integration-os-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Agent Infrastructure
- AI Agents
- Connectors
- Historical
- Integrations
- iPaaS
- MCP
- Rebrand
- Unified API
---
