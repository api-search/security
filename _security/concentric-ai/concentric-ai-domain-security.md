---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: concentric.ai
  spf: true
hosts:
- cert_expires: Sep 19 11:46:53 2026 GMT
  host: www.concentric.ai
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Concentric Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Concentric AI, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Concentric AI
provider_slug: concentric-ai
slug: concentric-ai-domain-security
source_filename: concentric-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.concentric.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 19 11:46:53 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: concentric.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/concentric-ai/refs/heads/main/security/concentric-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Security
- Data Security
- Data Security Posture Management
- Data Classification
- Data Access Governance
- Insider Risk
- Generative AI Security
- Compliance
---
