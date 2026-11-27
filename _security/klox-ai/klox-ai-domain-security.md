---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: klox.ai
  spf: true
hosts:
- cert_expires: Jan 24 05:02:05 2027 GMT
  host: klox.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Klox AI Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Klox AI, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Klox AI
provider_slug: klox-ai
slug: klox-ai-domain-security
source_filename: klox-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: klox.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 24 05:02:05 2027 GMT\n  hsts: false\ndomains:\n- domain: klox.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/klox-ai/security/klox-ai-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Artificial Intelligence
- Video Creation
- Platform
- Creative Tools
---
