---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: slang.ai
  spf: true
hosts:
- cert_expires: Sep 14 23:31:04 2026 GMT
  host: www.slang.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Slang Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Slang, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Slang
provider_slug: slang
slug: slang-domain-security
source_filename: slang-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.slang.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 23:31:04 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: slang.ai\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/slang/refs/heads/main/security/slang-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Ai
- Voice AI
- Conversational AI
- Restaurants
- Hospitality
- SaaS
---
