---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: heycactus.ai
  spf: false
hosts:
- cert_expires: Feb  3 05:50:42 2027 GMT
  host: heycactus.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Cactus Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cactus, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF absent, DMARC absent.'
provider_name: Cactus
provider_slug: heycactus-ai
slug: heycactus-ai-domain-security
source_filename: heycactus-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: heycactus.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  3 05:50:42 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: heycactus.ai\n  dnssec: true\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/heycactus-ai/security/heycactus-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC
tags:
- Artificial Intelligence
- Support
- Help Center
- Documentation
- Automation
- Company
---
