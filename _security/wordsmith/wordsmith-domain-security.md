---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: wordsmith.ai
  spf: true
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  dmarc: false
  dnssec: false
  domain: mintlify.app
  spf: false
hosts:
- cert_expires: Sep 12 21:29:19 2026 GMT
  host: www.wordsmith.ai
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 26 04:22:31 2026 GMT
  host: wordsmithai.mintlify.app
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 15 23:59:59 2026 GMT
  host: api.wordsmith.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Wordsmith Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Wordsmith, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Wordsmith
provider_slug: wordsmith
slug: wordsmith-domain-security
source_filename: wordsmith-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.wordsmith.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 12 21:29:19 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: wordsmithai.mintlify.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 26 04:22:31 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.wordsmith.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: wordsmith.ai\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: mintlify.app\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wordsmith/refs/heads/main/security/wordsmith-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Legal
- Legal Tech
- Legal AI
- In-House Legal
- General Counsel
- Contract Review
- Contract Lifecycle Management
- Document Generation
- Playbooks
- Templates
- AI Assistants
- AI Agents
- Agentic AI
- Slack
- Microsoft Teams
- Compliance
- Governance
- Risk
- Legal Engineering
- MCP
---
