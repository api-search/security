---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: regie.ai
  spf: true
hosts:
- cert_expires: Sep 28 12:31:52 2026 GMT
  host: www.regie.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Regieai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Regie.ai, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Regie.ai
provider_slug: regieai
slug: regieai-domain-security
source_filename: regieai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.regie.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 12:31:52 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: regie.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/regieai/refs/heads/main/security/regieai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Ai Apps
- Sales Engagement
- Sales AI
- Outbound
- Prospecting
- Revenue Operations
- AI Agents
---
