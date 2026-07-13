---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: sakana.ai
  spf: true
hosts:
- cert_expires: Sep 20 06:30:50 2026 GMT
  host: sakana.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 24 03:28:42 2026 GMT
  host: api.sakana.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Sakana Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Sakana AI, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Sakana AI
provider_slug: sakana-ai
slug: sakana-ai-domain-security
source_filename: sakana-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: sakana.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 06:30:50 2026 GMT\n  hsts: false\n- host: api.sakana.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 24 03:28:42 2026 GMT\n  hsts: null\ndomains:\n- domain: sakana.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sakana-ai/refs/heads/main/security/sakana-ai-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- AI
- LLM
- Research
- Foundation Models
- Multi-Agent
- Orchestration
---
