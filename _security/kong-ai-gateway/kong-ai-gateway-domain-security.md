---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: konghq.com
  spf: true
hosts:
- cert_expires: Dec 31 23:59:59 2026 GMT
  host: konghq.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 22 00:53:45 2026 GMT
  host: developer.konghq.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Kong Ai Gateway Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Kong AI Gateway, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Kong AI Gateway
provider_slug: kong-ai-gateway
slug: kong-ai-gateway-domain-security
source_filename: kong-ai-gateway-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: konghq.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 31 23:59:59 2026 GMT\n  hsts: false\n- host: developer.konghq.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 22 00:53:45 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: konghq.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kong-ai-gateway/refs/heads/main/security/kong-ai-gateway-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- AI Gateway
- LLM
- MCP
- A2A
- AI Governance
- Konnect
- Kong
---
