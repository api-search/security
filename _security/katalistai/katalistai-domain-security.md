---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: katalist.ai
  spf: true
hosts:
- cert_expires: Oct  1 20:08:56 2026 GMT
  host: katalist.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Katalistai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for KatalistAI, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: KatalistAI
provider_slug: katalistai
slug: katalistai-domain-security
source_filename: katalistai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: katalist.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 20:08:56 2026 GMT\n  hsts: null\ndomains:\n- domain: katalist.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/katalistai/refs/heads/main/security/katalistai-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Artificial Intelligence
- Generative AI
- Storyboarding
- Video
- Content Creation
- Filmmaking
- Creative Tools
- SaaS
---
