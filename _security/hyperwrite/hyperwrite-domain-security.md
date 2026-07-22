---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: hyperwriteai.com
  spf: true
hosts:
- cert_expires: Aug 17 04:43:45 2026 GMT
  host: www.hyperwriteai.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  3 09:29:54 2026 GMT
  host: app.hyperwriteai.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Hyperwrite Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for HyperWrite, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: HyperWrite
provider_slug: hyperwrite
slug: hyperwrite-domain-security
source_filename: hyperwrite-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.hyperwriteai.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 17 04:43:45 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: app.hyperwriteai.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  3 09:29:54 2026 GMT\n  hsts: false\ndomains:\n- domain: hyperwriteai.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hyperwrite/refs/heads/main/security/hyperwrite-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- AI
- Writing
- Assistant
- Agent
- Browser Automation
- Consumer
- Productivity
---
