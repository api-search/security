---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: lrclib.net
  spf: false
hosts:
- cert_expires: Jan 23 14:01:27 2027 GMT
  host: lrclib.net
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Lrclib Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for LRCLIB, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=reject).'
provider_name: LRCLIB
provider_slug: lrclib
slug: lrclib-domain-security
source_filename: lrclib-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: lrclib.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 23 14:01:27 2027 GMT\n  hsts: false\ndomains:\n- domain: lrclib.net\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/lrclib/security/lrclib-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Lyrics
- Music
- API
- OpenSource
---
