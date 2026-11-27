---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: ai-arena.ca
  spf: true
hosts:
- cert_expires: Jan 17 02:50:39 2027 GMT
  host: ai-arena.ca
  hsts: true
  hsts_max_age: 604800
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: AI Arena Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AI Arena, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: AI Arena
provider_slug: ai-arena-ca
slug: ai-arena-ca-domain-security
source_filename: ai-arena-ca-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ai-arena.ca\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 17 02:50:39 2027 GMT\n  hsts: true\n  hsts_max_age: 604800\ndomains:\n- domain: ai-arena.ca\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/ai-arena-ca/security/ai-arena-ca-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Music
- Artificial Intelligence
- Discovery
- Community
- Independent
---
