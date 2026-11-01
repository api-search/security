---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: raga.ai
  spf: true
hosts:
- cert_expires: Dec  1 15:32:33 2026 GMT
  host: raga.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Raga Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for RagaAI, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: RagaAI
provider_slug: raga
slug: raga-domain-security
source_filename: raga-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: raga.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  1 15:32:33 2026 GMT\n  hsts: false\ndomains:\n- domain: raga.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/raga/security/raga-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Artificial Intelligence
- Natural Language Processing
- Platform
- Developer Tools
---
