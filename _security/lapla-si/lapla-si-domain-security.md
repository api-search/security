---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: lapla.si
  spf: true
hosts:
- cert_expires: Jan 11 09:38:54 2027 GMT
  host: lapla.si
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Lapla Si Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for lapla-si, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: lapla-si
provider_slug: lapla-si
slug: lapla-si-domain-security
source_filename: lapla-si-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: lapla.si\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 11 09:38:54 2027 GMT\n  hsts: false\ndomains:\n- domain: lapla.si\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/lapla-si/security/lapla-si-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- AI
- macOS
- Productivity
- Workspace
- Dictation
---
