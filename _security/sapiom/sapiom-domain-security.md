---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: sapiom.ai
  spf: true
hosts:
- cert_expires: Aug 24 02:59:04 2026 GMT
  host: www.sapiom.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 26 23:10:48 2026 GMT
  host: docs.sapiom.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 25 08:28:26 2026 GMT
  host: api.sapiom.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Sapiom Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Sapiom, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Sapiom
provider_slug: sapiom
slug: sapiom-domain-security
source_filename: sapiom-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.sapiom.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 24 02:59:04 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.sapiom.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 26 23:10:48 2026 GMT\n  hsts: false\n- host: api.sapiom.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 25 08:28:26 2026 GMT\n  hsts: false\ndomains:\n- domain: sapiom.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sapiom/refs/heads/main/security/sapiom-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Ai
- AI Agents
- Agent Infrastructure
- Model Context Protocol
- API Gateway
- Payments
- Agentic Commerce
- Developer Tools
- SDK
---
