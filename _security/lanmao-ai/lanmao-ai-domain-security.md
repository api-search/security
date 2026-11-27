---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: lanmao.ai
  spf: true
hosts:
- cert_expires: Feb  3 18:08:57 2027 GMT
  host: lanmao.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Lanmao AI Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Lanmao AI, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Lanmao AI
provider_slug: lanmao-ai
slug: lanmao-ai-domain-security
source_filename: lanmao-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-14'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: lanmao.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  3 18:08:57 2027 GMT\n  hsts: false\ndomains:\n- domain: lanmao.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/lanmao-ai/security/lanmao-ai-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Artificial Intelligence
- Directory
- FreeCredits
- Developer Tools
- Marketplace
---
