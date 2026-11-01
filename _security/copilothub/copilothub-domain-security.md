---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: devv.ai
  spf: true
hosts:
- cert_expires: Nov 20 15:19:35 2026 GMT
  host: devv.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Copilothub Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Copilothub, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Copilothub
provider_slug: copilothub
slug: copilothub-domain-security
source_filename: copilothub-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: devv.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 20 15:19:35 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: devv.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/copilothub/security/copilothub-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- AI
- CodingAgent
- DeveloperTools
- Startup
---
