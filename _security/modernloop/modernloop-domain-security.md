---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: modernloop.io
  spf: true
hosts:
- cert_expires: Sep 29 09:09:25 2026 GMT
  host: www.modernloop.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Modernloop Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ModernLoop, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: ModernLoop
provider_slug: modernloop
slug: modernloop-domain-security
source_filename: modernloop-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.modernloop.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 09:09:25 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: modernloop.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/modernloop/refs/heads/main/security/modernloop-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Hr Tech
- Recruiting
- Interview Scheduling
- Talent Acquisition
- Hiring
- AI Agents
- SaaS
---
