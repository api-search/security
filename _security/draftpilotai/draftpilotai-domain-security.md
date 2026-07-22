---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: draftpilot.ai
  spf: false
hosts:
- cert_expires: Oct 16 19:21:10 2026 GMT
  host: draftpilot.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Draftpilotai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for DraftPilot.ai, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF absent, DMARC present (p=quarantine).'
provider_name: DraftPilot.ai
provider_slug: draftpilotai
slug: draftpilotai-domain-security
source_filename: draftpilotai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: draftpilot.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 16 19:21:10 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: draftpilot.ai\n  dnssec: true\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/draftpilotai/refs/heads/main/security/draftpilotai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Legal
- Legal Tech
- Contracts
- Contract Review
- Contract Redlining
- Artificial Intelligence
- Document Automation
- Microsoft Word
---
