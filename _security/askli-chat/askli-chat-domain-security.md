---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: askli.chat
  spf: true
hosts:
- cert_expires: Dec  6 03:46:10 2026 GMT
  host: askli.chat
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Askli Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Askli, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Askli
provider_slug: askli-chat
slug: askli-chat-domain-security
source_filename: askli-chat-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: askli.chat\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  6 03:46:10 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: askli.chat\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/askli-chat/security/askli-chat-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Artificial Intelligence
- User Research
- Market Validation
- Product Development
- Software-as-a-Service
---
