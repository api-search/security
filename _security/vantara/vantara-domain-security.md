---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: getmilana.ai
  spf: true
hosts:
- cert_expires: Oct  1 03:27:22 2026 GMT
  host: getmilana.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Vantara Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Milana, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Milana
provider_slug: vantara
slug: vantara-domain-security
source_filename: vantara-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: getmilana.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 03:27:22 2026 GMT\n  hsts: false\ndomains:\n- domain: getmilana.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vantara/refs/heads/main/security/vantara-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- AI
- Session Replay
- Product Analytics
- Developer Tools
- Agents
- SDK
---
