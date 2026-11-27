---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: funlet.ai
  spf: true
hosts:
- cert_expires: Dec 11 06:50:50 2026 GMT
  host: funlet.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Funlet Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Funlet, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Funlet
provider_slug: funlet-ai
slug: funlet-ai-domain-security
source_filename: funlet-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-08'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: funlet.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 11 06:50:50 2026 GMT\n  hsts: false\ndomains:\n- domain: funlet.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/funlet-ai/security/funlet-ai-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Coordination
- AI Agents
---
