---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: norm.ai
  spf: true
hosts:
- cert_expires: Sep 14 02:17:06 2026 GMT
  host: www.norm.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Norm Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Norm Ai, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Norm Ai
provider_slug: norm-ai
slug: norm-ai-domain-security
source_filename: norm-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.norm.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 02:17:06 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: norm.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/norm-ai/refs/heads/main/security/norm-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Ai Apps
- Legal
- Compliance
- AI Agents
- RegTech
- Governance
---
