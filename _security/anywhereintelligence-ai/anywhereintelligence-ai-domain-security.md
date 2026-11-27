---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: anywhereintelligence.ai
  spf: true
hosts:
- cert_expires: Dec 16 07:07:55 2026 GMT
  host: anywhereintelligence.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Anywhere Intelligence Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Anywhere Intelligence, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Anywhere Intelligence
provider_slug: anywhereintelligence-ai
slug: anywhereintelligence-ai-domain-security
source_filename: anywhereintelligence-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: anywhereintelligence.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 16 07:07:55 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: anywhereintelligence.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/anywhereintelligence-ai/security/anywhereintelligence-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Artificial Intelligence
- Personal AI
- Privacy
- Decentralization
- Mac
---
