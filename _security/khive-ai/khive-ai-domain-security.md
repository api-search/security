---
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: khive.ai
  spf: true
hosts:
- cert_expires: Jan 28 19:36:08 2027 GMT
  host: khive.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: khive AI Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for khive AI, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: khive AI
provider_slug: khive-ai
slug: khive-ai-domain-security
source_filename: khive-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: khive.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 28 19:36:08 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: khive.ai\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/khive-ai/security/khive-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Artificial Intelligence
- Cognitive Infrastructure
- Memory
- Knowledge Graph
- Multi-Agent
---
