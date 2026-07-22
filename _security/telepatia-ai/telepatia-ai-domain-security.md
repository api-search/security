---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: telepatia.ai
  spf: true
hosts:
- cert_expires: Aug 26 00:01:05 2026 GMT
  host: www.telepatia.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Telepatia Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Telepatia AI, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Telepatia AI
provider_slug: telepatia-ai
slug: telepatia-ai-domain-security
source_filename: telepatia-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.telepatia.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 26 00:01:05 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: telepatia.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/telepatia-ai/refs/heads/main/security/telepatia-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Healthcare
- Artificial Intelligence
- Clinical Documentation
- Medical Scribe
- Electronic Health Records
- Latin America
- Clinical Decision Support
---
