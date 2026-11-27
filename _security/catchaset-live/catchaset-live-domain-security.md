---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: catchaset.live
  spf: true
hosts:
- cert_expires: Jan 12 21:59:04 2027 GMT
  host: catchaset.live
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: CatchaSet Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CatchaSet, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: CatchaSet
provider_slug: catchaset-live
slug: catchaset-live-domain-security
source_filename: catchaset-live-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: catchaset.live\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 12 21:59:04 2027 GMT\n  hsts: null\ndomains:\n- domain: catchaset.live\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/catchaset-live/security/catchaset-live-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Music
- Live Events
- Discovery
- Austin
- Entertainment
---
