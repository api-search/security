---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: arbiter.ai
  spf: true
hosts:
- cert_expires: Nov 27 16:39:53 2026 GMT
  host: www.arbiter.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Arbiter Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Arbiter AI, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Arbiter AI
provider_slug: arbiter-ai
slug: arbiter-ai-domain-security
source_filename: arbiter-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.arbiter.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 27 16:39:53 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: arbiter.ai\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/arbiter-ai/refs/heads/main/security/arbiter-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Healthcare
- AI
- CareOrchestration
- PopulationHealth
- Platform
---
