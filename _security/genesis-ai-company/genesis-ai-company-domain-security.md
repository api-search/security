---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: genesis-ai.company
  spf: true
hosts:
- cert_expires: Dec  7 23:17:44 2026 GMT
  host: genesis-ai.company
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Genesis Ai Company Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Genesis Ai, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Genesis Ai
provider_slug: genesis-ai-company
slug: genesis-ai-company-domain-security
source_filename: genesis-ai-company-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: genesis-ai.company\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  7 23:17:44 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: genesis-ai.company\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/genesis-ai-company/security/genesis-ai-company-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- AI
- Startup
- GenerativeAI
- Platform
---
