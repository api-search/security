---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: reaper.fm
  spf: true
hosts:
- cert_expires: Dec 15 17:13:55 2026 GMT
  host: www.reaper.fm
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Cockos Reaper Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for REAPER, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: REAPER
provider_slug: cockos-reaper
slug: cockos-reaper-domain-security
source_filename: cockos-reaper-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.reaper.fm\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 15 17:13:55 2026 GMT\n  hsts: false\ndomains:\n- domain: reaper.fm\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/cockos-reaper/security/cockos-reaper-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Audio
- Digital Audio Workstation
- Music Production
- Windows
- macOS
- Linux
---
