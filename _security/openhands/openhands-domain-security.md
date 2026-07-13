---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: openhands.dev
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: all-hands.dev
  spf: false
hosts:
- cert_expires: Aug 20 19:59:36 2026 GMT
  host: www.openhands.dev
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 23 08:44:38 2026 GMT
  host: app.all-hands.dev
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Openhands Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for OpenHands, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: OpenHands
provider_slug: openhands
slug: openhands-domain-security
source_filename: openhands-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.openhands.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 20 19:59:36 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: app.all-hands.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 23 08:44:38 2026 GMT\n  hsts: false\ndomains:\n- domain: openhands.dev\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: all-hands.dev\n  dnssec: true\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/openhands/refs/heads/main/security/openhands-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- AI
- Agents
- Autonomous
- Open Source
- Developer Tools
- Software Engineering
- Code Generation
---
