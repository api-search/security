---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: cairn.ink
  spf: true
hosts:
- cert_expires: Jan 30 13:12:47 2027 GMT
  host: cairn.ink
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Cairn Ink Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cairn, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Cairn
provider_slug: cairn-ink
slug: cairn-ink-domain-security
source_filename: cairn-ink-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cairn.ink\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 30 13:12:47 2027 GMT\n  hsts: false\ndomains:\n- domain: cairn.ink\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/cairn-ink/security/cairn-ink-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Artificial Intelligence
- Memory
- Platform
- Collaboration
---
