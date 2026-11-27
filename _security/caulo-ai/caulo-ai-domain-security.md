---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: caulo.ai
  spf: true
hosts:
- cert_expires: Jan  2 21:46:10 2027 GMT
  host: caulo.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Caulo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Caulo, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Caulo
provider_slug: caulo-ai
slug: caulo-ai-domain-security
source_filename: caulo-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: caulo.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  2 21:46:10 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: caulo.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/caulo-ai/security/caulo-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Artificial Intelligence
- Social
- Networks
- Agents
- Platform
---
