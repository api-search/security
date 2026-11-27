---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: avva.chat
  spf: true
hosts:
- cert_expires: Jan 30 17:25:35 2027 GMT
  host: avva.chat
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: avva Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for avva, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: avva
provider_slug: avva-chat
slug: avva-chat-domain-security
source_filename: avva-chat-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: avva.chat\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 30 17:25:35 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: avva.chat\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/avva-chat/security/avva-chat-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Artificial Intelligence
- DecisionModel
- Expertise
- Platform
- Barcelona
---
