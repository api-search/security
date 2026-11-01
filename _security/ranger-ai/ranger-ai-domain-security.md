---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: rangerx.ai
  spf: true
hosts:
- cert_expires: Jan 10 08:42:41 2027 GMT
  host: rangerx.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Ranger Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ranger AI, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Ranger AI
provider_slug: ranger-ai
slug: ranger-ai-domain-security
source_filename: ranger-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: rangerx.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 10 08:42:41 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: rangerx.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/ranger-ai/security/ranger-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- AI
- Industrial Engineering
- Procurement
- Document Automation
---
