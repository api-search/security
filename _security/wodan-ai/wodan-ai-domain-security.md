---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: wodan.ai
  spf: true
hosts:
- cert_expires: Dec  7 07:42:08 2026 GMT
  host: wodan.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Wodan Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Wodan AI, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Wodan AI
provider_slug: wodan-ai
slug: wodan-ai-domain-security
source_filename: wodan-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: wodan.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  7 07:42:08 2026 GMT\n  hsts: false\ndomains:\n- domain: wodan.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/wodan-ai/security/wodan-ai-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- AI
- Zero-Trust
- Encryption
- Data-Privacy
- Financial-Services
---
