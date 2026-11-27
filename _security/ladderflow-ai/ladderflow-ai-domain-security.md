---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: ladderflow.ai
  spf: false
hosts:
- cert_expires: Jan 12 09:38:04 2027 GMT
  host: ladderflow.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Ladder Flow Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ladder Flow, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=quarantine).'
provider_name: Ladder Flow
provider_slug: ladderflow-ai
slug: ladderflow-ai-domain-security
source_filename: ladderflow-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-14'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ladderflow.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 12 09:38:04 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: ladderflow.ai\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/ladderflow-ai/security/ladderflow-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Artificial Intelligence
- Content Generation
- Social Media
- B2B
- Podcasts
---
