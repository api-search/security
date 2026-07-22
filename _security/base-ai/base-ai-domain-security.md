---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: base.ai
  spf: true
hosts:
- cert_expires: Sep  4 01:22:26 2026 GMT
  host: base.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Base Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Base Ai, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Base Ai
provider_slug: base-ai
slug: base-ai-domain-security
source_filename: base-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: base.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  4 01:22:26 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: base.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/base-ai/refs/heads/main/security/base-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Artificial Intelligence
- Customer-Led Growth
- Customer Success
- Customer Marketing
- Advocacy
- RevOps
- SaaS
---
