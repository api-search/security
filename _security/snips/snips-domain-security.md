---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: snips.ai
  spf: true
hosts:
- cert_expires: Jan 30 23:59:59 2027 GMT
  host: snips.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Snips Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Snips, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Snips
provider_slug: snips
slug: snips-domain-security
source_filename: snips-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: snips.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 30 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: snips.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/snips/refs/heads/main/security/snips-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Voice
- Artificial Intelligence
- Natural Language Understanding
- Voice Assistant
- On-Device AI
- Privacy
- Acquired
---
