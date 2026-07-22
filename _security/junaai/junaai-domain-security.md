---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: juna.ai
  spf: true
hosts:
- cert_expires: Oct  3 19:44:43 2026 GMT
  host: juna.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Junaai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Juna.ai, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Juna.ai
provider_slug: junaai
slug: junaai-domain-security
source_filename: junaai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: juna.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 19:44:43 2026 GMT\n  hsts: false\ndomains:\n- domain: juna.ai\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/junaai/refs/heads/main/security/junaai-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Ai
- Industrial AI
- Manufacturing
- AI Agents
- Process Control
- Energy Efficiency
- Sustainability
- Enterprise
---
