---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: powerline.ai
  spf: true
hosts:
- cert_expires: Jan 25 02:31:08 2027 GMT
  host: powerline.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Powerline Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for powerline-ai, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: powerline-ai
provider_slug: powerline-ai
slug: powerline-ai-domain-security
source_filename: powerline-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: powerline.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 25 02:31:08 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: powerline.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/powerline-ai/security/powerline-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- AI
- APIs
- Automation
- Email
- Productivity
---
