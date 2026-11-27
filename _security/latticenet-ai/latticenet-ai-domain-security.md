---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: latticenet.ai
  spf: true
hosts:
- cert_expires: Jan 30 05:19:44 2027 GMT
  host: latticenet.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: LatticeNet Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for LatticeNet, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: LatticeNet
provider_slug: latticenet-ai
slug: latticenet-ai-domain-security
source_filename: latticenet-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-14'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: latticenet.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 30 05:19:44 2027 GMT\n  hsts: false\ndomains:\n- domain: latticenet.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/latticenet-ai/security/latticenet-ai-domain-security.yml
summary_line: TLSv1.3
tags:
- Artificial Intelligence
- Publishing
- Agents
- Platform
- API-First
---
