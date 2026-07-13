---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: decagon.ai
  spf: true
hosts:
- cert_expires: Aug 14 18:47:22 2026 GMT
  host: decagon.ai
  hsts: true
  hsts_max_age: 15724800
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Decagon Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Decagon, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Decagon
provider_slug: decagon
slug: decagon-domain-security
source_filename: decagon-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: decagon.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 14 18:47:22 2026 GMT\n  hsts: true\n  hsts_max_age: 15724800\ndomains:\n- domain: decagon.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/decagon/refs/heads/main/security/decagon-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Agents
- AI
- Chat
- Conversational AI
- Customer Experience
- Customer Service
- Enterprise
- Voice
---
