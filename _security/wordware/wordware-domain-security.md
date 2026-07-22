---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: wordware.ai
  spf: true
hosts:
- cert_expires: Oct  3 17:55:12 2026 GMT
  host: wordware.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 12 11:40:41 2026 GMT
  host: docs.wordware.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 25 20:31:04 2026 GMT
  host: app.wordware.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Wordware Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Wordware, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Wordware
provider_slug: wordware
slug: wordware-domain-security
source_filename: wordware-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: wordware.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 17:55:12 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.wordware.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 12 11:40:41 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: app.wordware.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 20:31:04 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: wordware.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wordware/refs/heads/main/security/wordware-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Artificial Intelligence
- AI Agents
- LLM
- Prompt Engineering
- Workflow Automation
- No Code
- Company
---
