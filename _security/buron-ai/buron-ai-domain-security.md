---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: buron.ai
  spf: true
hosts:
- cert_expires: Dec  2 10:09:05 2026 GMT
  host: buron.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Buron Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for buron-ai, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: buron-ai
provider_slug: buron-ai
slug: buron-ai-domain-security
source_filename: buron-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: buron.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  2 10:09:05 2026 GMT\n  hsts: null\ndomains:\n- domain: buron.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/buron-ai/security/buron-ai-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
---
