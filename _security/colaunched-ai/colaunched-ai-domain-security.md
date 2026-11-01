---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: colaunched.ai
  spf: true
hosts:
- cert_expires: Dec  3 15:20:29 2026 GMT
  host: colaunched.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Colaunched Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for colaunched-ai, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: colaunched-ai
provider_slug: colaunched-ai
slug: colaunched-ai-domain-security
source_filename: colaunched-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: colaunched.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  3 15:20:29 2026 GMT\n  hsts: false\ndomains:\n- domain: colaunched.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/colaunched-ai/security/colaunched-ai-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Business
- Startup
- Idea-Generation
- Market-Research
---
