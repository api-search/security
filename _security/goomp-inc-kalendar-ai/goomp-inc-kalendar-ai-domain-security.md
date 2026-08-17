---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: oncockpit.ai
  spf: true
hosts:
- cert_expires: Oct  3 02:21:56 2026 GMT
  host: oncockpit.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  3 02:21:56 2026 GMT
  host: api.oncockpit.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Goomp Inc Kalendar Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Goomp Inc, Kalendar AI, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Goomp Inc, Kalendar AI
provider_slug: goomp-inc-kalendar-ai
slug: goomp-inc-kalendar-ai-domain-security
source_filename: goomp-inc-kalendar-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: oncockpit.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 02:21:56 2026 GMT\n  hsts: false\n- host: api.oncockpit.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 02:21:56 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: oncockpit.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/goomp-inc-kalendar-ai/refs/heads/main/security/goomp-inc-kalendar-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Artificial Intelligence
- Sales
- Sales Automation
- Outbound
- Lead Generation
- Scheduling
- Agents
- Email
- CRM
---
