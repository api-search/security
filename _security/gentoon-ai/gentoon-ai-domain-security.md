---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: gentoon.ai
  spf: true
hosts:
- cert_expires: Jan  2 08:02:37 2027 GMT
  host: gentoon.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: GenToon Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for GenToon, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: GenToon
provider_slug: gentoon-ai
slug: gentoon-ai-domain-security
source_filename: gentoon-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-09'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: gentoon.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  2 08:02:37 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: gentoon.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/gentoon-ai/security/gentoon-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Artificial Intelligence
- Webtoon
- Creative
- Platform
- GenToon
---
