---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: kadenza.ai
  spf: false
hosts:
- cert_expires: Jan 18 22:19:06 2027 GMT
  host: kadenza.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Kadenza Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Kadenza, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: Kadenza
provider_slug: kadenza-ai
slug: kadenza-ai-domain-security
source_filename: kadenza-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: kadenza.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 18 22:19:06 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: kadenza.ai\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/kadenza-ai/security/kadenza-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Software-as-a-Service
- Personal Branding
- Artificial Intelligence
- Content Creation
- Marketing
---
