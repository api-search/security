---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: objekts.ai
  spf: true
hosts:
- cert_expires: Jan 29 04:31:18 2027 GMT
  host: objekts.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: objekts Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for objekts, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: objekts
provider_slug: objekts-ai
slug: objekts-ai-domain-security
source_filename: objekts-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: objekts.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 29 04:31:18 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: objekts.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/objekts-ai/security/objekts-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Visual
- Production
- Advertising
- Animation
- VFX
---
