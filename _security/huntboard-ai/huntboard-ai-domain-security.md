---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: huntboard.ai
  spf: true
hosts:
- cert_expires: Jan  4 12:17:14 2027 GMT
  host: huntboard.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: HuntBoard Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for HuntBoard, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: HuntBoard
provider_slug: huntboard-ai
slug: huntboard-ai-domain-security
source_filename: huntboard-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: huntboard.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  4 12:17:14 2027 GMT\n  hsts: false\ndomains:\n- domain: huntboard.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/huntboard-ai/security/huntboard-ai-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Job Search
- ATS Integration
- Job Matching
---
