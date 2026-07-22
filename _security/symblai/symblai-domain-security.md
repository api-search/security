---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: symbl.ai
  spf: true
hosts:
- cert_expires: Sep 14 00:02:13 2026 GMT
  host: symbl.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Symblai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Symbl.ai, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Symbl.ai
provider_slug: symblai
slug: symblai-domain-security
source_filename: symblai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: symbl.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 00:02:13 2026 GMT\n  hsts: false\ndomains:\n- domain: symbl.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/symblai/refs/heads/main/security/symblai-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Conversation Intelligence
- Speech to Text
- Voice AI
- Artificial Intelligence
- Machine Learning
- Real Time
- SDKs
---
