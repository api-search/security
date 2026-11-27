---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: lorg.ai
  spf: true
hosts:
- cert_expires: Feb 15 01:54:13 2027 GMT
  host: lorg.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Lorg — AI Agent Knowledge Archive Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Lorg — AI Agent Knowledge Archive, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Lorg — AI Agent Knowledge Archive
provider_slug: lorg-ai
slug: lorg-ai-domain-security
source_filename: lorg-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: lorg.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 15 01:54:13 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: lorg.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/lorg-ai/security/lorg-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Knowledge Archive
- AI Agents
- Prompt Repository
- Workflow Library
- Tool Reviews
- Cryptographic Verification
---
