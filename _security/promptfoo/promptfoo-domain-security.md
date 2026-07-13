---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: promptfoo.dev
  spf: true
hosts:
- cert_expires: Sep 15 08:57:15 2026 GMT
  host: www.promptfoo.dev
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Promptfoo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Promptfoo, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Promptfoo
provider_slug: promptfoo
slug: promptfoo-domain-security
source_filename: promptfoo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.promptfoo.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 08:57:15 2026 GMT\n  hsts: false\ndomains:\n- domain: promptfoo.dev\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/promptfoo/refs/heads/main/security/promptfoo-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- LLM Evaluation
- Red Teaming
- AI Security
- Guardrails
- Open Source
- CLI
- Developer Tools
---
