---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: noveum.ai
  spf: true
hosts:
- cert_expires: Dec 22 14:19:55 2026 GMT
  host: noveum.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Noveum Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for noveum-ai, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: noveum-ai
provider_slug: noveum-ai
slug: noveum-ai-domain-security
source_filename: noveum-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: noveum.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 22 14:19:55 2026 GMT\n  hsts: false\ndomains:\n- domain: noveum.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/noveum-ai/security/noveum-ai-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- AI
- Evaluation
- Observability
- Enterprise
---
