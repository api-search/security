---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: voyce.me
  spf: true
hosts:
- cert_expires: Feb  4 23:59:59 2027 GMT
  host: voyce.me
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Voyceme Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for VoyceMe, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: VoyceMe
provider_slug: voyceme
slug: voyceme-domain-security
source_filename: voyceme-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: voyce.me\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Feb  4 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: voyce.me\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/voyceme/refs/heads/main/security/voyceme-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- Company
- Manga
- Webtoons
- Web Novels
- Comics
- Publishing
- Creators
- GraphQL
- AI Characters
- Entertainment
- Media
---
