---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: boardroom-ai.ae
  spf: true
hosts:
- cert_expires: Jan  5 22:40:24 2027 GMT
  host: boardroom-ai.ae
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Boardroom AI Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Boardroom AI, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Boardroom AI
provider_slug: boardroom-ai-ae
slug: boardroom-ai-ae-domain-security
source_filename: boardroom-ai-ae-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: boardroom-ai.ae\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  5 22:40:24 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: boardroom-ai.ae\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/boardroom-ai-ae/security/boardroom-ai-ae-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Artificial Intelligence
- Revenue
- CRM
- United Arab Emirates
- Software-as-a-Service
---
