---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: botguard.io
  spf: true
hosts:
- cert_expires: Dec 13 06:27:28 2026 GMT
  host: botguard.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Botguard Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Botguard, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Botguard
provider_slug: botguard
slug: botguard-domain-security
source_filename: botguard-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-03'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: botguard.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 13 06:27:28 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: botguard.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/botguard/refs/heads/main/security/botguard-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Artificial Intelligence
- Security
- Anti-Prompt-Injection
- Enterprise
---
