---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: ai-gist.com
  spf: false
hosts:
- cert_expires: Dec  4 13:18:11 2026 GMT
  host: ai-gist.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Aigist Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Aigist, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Aigist
provider_slug: ai-gist-com
slug: ai-gist-com-domain-security
source_filename: ai-gist-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ai-gist.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  4 13:18:11 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: ai-gist.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/ai-gist-com/security/ai-gist-com-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Artificial Intelligence
- Publishing
- LLM
- Content Sharing
- Platform
---
