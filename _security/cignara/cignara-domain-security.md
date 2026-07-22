---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: cignara.com
  spf: true
hosts:
- cert_expires: Sep  4 05:37:25 2026 GMT
  host: cignara.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Cignara Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cignara, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Cignara
provider_slug: cignara
slug: cignara-domain-security
source_filename: cignara-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cignara.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  4 05:37:25 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: cignara.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cignara/refs/heads/main/security/cignara-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Artificial Intelligence
- Conversational AI
- Customer Support
- Voice Agents
- Chat Agents
- Contact Center
- Enterprise AI
- AI Agents
---
