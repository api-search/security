---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: fiberfinder.ai
  spf: true
hosts:
- cert_expires: Dec 20 09:57:05 2026 GMT
  host: fiberfinder.ai
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: FiberFinder Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for FiberFinder, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: FiberFinder
provider_slug: fiberfinder-ai
slug: fiberfinder-ai-domain-security
source_filename: fiberfinder-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-07'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: fiberfinder.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 20 09:57:05 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: fiberfinder.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/fiberfinder-ai/security/fiberfinder-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Fiber
- Internet
- Broadband
- Artificial Intelligence
- Consumer
---
