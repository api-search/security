---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: cequence.ai
  spf: true
hosts:
- cert_expires: Sep 26 17:38:02 2026 GMT
  host: www.cequence.ai
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  6 21:09:33 2026 GMT
  host: docs.aigateway.cequence.ai
  hsts: true
  hsts_max_age: 31556926
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 12 17:18:56 2026 GMT
  host: aigateway.cequence.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Cequence Security Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cequence Security, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Cequence Security
provider_slug: cequence-security
slug: cequence-security-domain-security
source_filename: cequence-security-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.cequence.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 17:38:02 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\n- host: docs.aigateway.cequence.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  6 21:09:33 2026 GMT\n  hsts: true\n  hsts_max_age: 31556926\n- host: aigateway.cequence.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 12 17:18:56 2026 GMT\n  hsts: false\ndomains:\n- domain: cequence.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cequence-security/refs/heads/main/security/cequence-security-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- api-security
- ai-gateway
- MCP
- agentic-ai
- bot-management
- api-discovery
- api-governance
- fraud-detection
- waap
- Cybersecurity
- api-testing
- agent-native
---
