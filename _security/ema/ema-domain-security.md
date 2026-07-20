---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: ema.co
  spf: true
hosts:
- cert_expires: Sep 21 22:04:17 2026 GMT
  host: ema.co
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ema Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ema, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Ema
provider_slug: ema
slug: ema-domain-security
source_filename: ema-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ema.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 22:04:17 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: ema.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ema/refs/heads/main/security/ema-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- AI
- Agents
- AI Employees
- Automation
- Enterprise
- Workflow Automation
- Conversational AI
---
