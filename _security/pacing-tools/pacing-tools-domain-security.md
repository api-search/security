---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: pacing.tools
  spf: true
hosts:
- cert_expires: Dec 22 07:51:40 2026 GMT
  host: pacing.tools
  hsts: true
  hsts_max_age: 604800
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Pacing Tools Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Pacing Tools, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Pacing Tools
provider_slug: pacing-tools
slug: pacing-tools-domain-security
source_filename: pacing-tools-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: pacing.tools\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 22 07:51:40 2026 GMT\n  hsts: true\n  hsts_max_age: 604800\ndomains:\n- domain: pacing.tools\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/pacing-tools/security/pacing-tools-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Fitness
- Artificial Intelligence
- Training Data
- Sports
- Integration
---
