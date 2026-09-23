---
api_specs:
- filename: servghost-agent-api-openapi.yml
  format: yaml
  label: ServGhost Agent API
  slug: servghost-agent-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/servghost-agent-api/refs/heads/main/openapi/servghost-agent-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: servghost.com
  spf: true
hosts:
- cert_expires: Dec 13 07:25:07 2026 GMT
  host: servghost.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Servghost Agent Api Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ServGhost Agent API, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: ServGhost Agent API
provider_slug: servghost-agent-api
slug: servghost-agent-api-domain-security
source_filename: servghost-agent-api-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: servghost.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 13 07:25:07 2026 GMT\n  hsts: false\ndomains:\n- domain: servghost.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/servghost-agent-api/refs/heads/main/security/servghost-agent-api-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Cloud Infrastructure
- VPS hosting
- Dedicated Servers
- GPU Compute
- AI Compute
- Domain Registration
- Privacy
- anonymous hosting
- offshore hosting
- Crypto Payments
- agent-native
- MCP
- x402
---
