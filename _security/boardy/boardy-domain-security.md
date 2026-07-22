---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: boardy.ai
  spf: true
hosts:
- cert_expires: Sep 20 21:04:50 2026 GMT
  host: www.boardy.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Boardy Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Boardy, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Boardy
provider_slug: boardy
slug: boardy-domain-security
source_filename: boardy-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.boardy.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 21:04:50 2026 GMT\n  hsts: false\ndomains:\n- domain: boardy.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/boardy/refs/heads/main/security/boardy-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Ai
- Artificial Intelligence
- Networking
- Professional Networking
- Introductions
- AI Agent
- Voice Agent
- Superconnector
---
