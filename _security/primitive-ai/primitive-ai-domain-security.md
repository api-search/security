---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: prai.tech
  spf: true
hosts:
- host: prai.tech
  https: false
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Primitive Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Primitive AI, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Primitive AI
provider_slug: primitive-ai
slug: primitive-ai-domain-security
source_filename: primitive-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-24'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: prai.tech\n  https: false\ndomains:\n- domain: prai.tech\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/primitive-ai/security/primitive-ai-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Company
---
