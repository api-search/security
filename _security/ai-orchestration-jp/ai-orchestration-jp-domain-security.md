---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: ai-orchestration.jp
  spf: true
hosts:
- cert_expires: Jan 22 14:15:07 2027 GMT
  host: ai-orchestration.jp
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: AI Orchestration Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AI Orchestration, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: AI Orchestration
provider_slug: ai-orchestration-jp
slug: ai-orchestration-jp-domain-security
source_filename: ai-orchestration-jp-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ai-orchestration.jp\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 22 14:15:07 2027 GMT\n  hsts: false\ndomains:\n- domain: ai-orchestration.jp\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/ai-orchestration-jp/security/ai-orchestration-jp-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Artificial Intelligence
- Consulting
- Japan
- Enterprise AI
- Integration
---
