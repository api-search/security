---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: kloudy.ai
  spf: true
hosts:
- cert_expires: Apr 15 23:59:59 2027 GMT
  host: kloudy.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Kloudy AI Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Kloudy AI, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Kloudy AI
provider_slug: kloudy-ai
slug: kloudy-ai-domain-security
source_filename: kloudy-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: kloudy.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Apr 15 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: kloudy.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/kloudy-ai/security/kloudy-ai-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Artificial Intelligence
- BotPlatform
- Automation
- Open Source
- WaterSaving
---
