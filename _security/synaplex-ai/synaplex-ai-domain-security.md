---
description: ''
domains:
- caa: []
  dmarc: false
  dns_aid:
    checked: '2026-11-25'
    published: false
  dnssec: false
  domain: synaplex.ai
  spf: true
hosts:
- cert_expires: Feb  5 20:47:27 2027 GMT
  host: synaplex.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Synaplex Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Synaplex, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Synaplex
provider_slug: synaplex-ai
slug: synaplex-ai-domain-security
source_filename: synaplex-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: synaplex.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  5 20:47:27 2027 GMT\n  hsts: false\ndomains:\n- domain: synaplex.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n  dns_aid:\n    checked: '2026-11-25'\n    published: false\n"
source_yaml_url: https://artifacts.apis.io/synaplex-ai/security/synaplex-ai-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Knowledge
- Research
- Platform
- OpenData
---
