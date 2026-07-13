---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: aider.chat
  spf: false
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: anthropic.com
  spf: true
hosts:
- cert_expires: Sep 26 20:23:51 2026 GMT
  host: aider.chat
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 17 19:48:08 2026 GMT
  host: docs.anthropic.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Conventions Md Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CONVENTIONS.md, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF absent, DMARC absent.'
provider_name: CONVENTIONS.md
provider_slug: conventions-md
slug: conventions-md-domain-security
source_filename: conventions-md-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: aider.chat\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 20:23:51 2026 GMT\n  hsts: false\n- host: docs.anthropic.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 17 19:48:08 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: aider.chat\n  dnssec: true\n  caa: []\n  spf: false\n  dmarc: false\n- domain: anthropic.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/conventions-md/refs/heads/main/security/conventions-md-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- AI Coding
- Aider
- Best Practices
- Coding Standards
- Conventions
- Developer Workflow
- Documentation
- Markdown
- Project Configuration
---
