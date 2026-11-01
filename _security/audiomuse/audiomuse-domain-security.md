---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: audiomuse.ai
  spf: true
hosts:
- cert_expires: Dec  8 01:21:04 2026 GMT
  host: audiomuse.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Audiomuse Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AudioMuse-AI, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: AudioMuse-AI
provider_slug: audiomuse
slug: audiomuse-domain-security
source_filename: audiomuse-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: audiomuse.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  8 01:21:04 2026 GMT\n  hsts: false\ndomains:\n- domain: audiomuse.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/audiomuse/security/audiomuse-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Music
- AI
- OpenSource
- Self-Hosted
- Playlist
- AudioAnalysis
---
