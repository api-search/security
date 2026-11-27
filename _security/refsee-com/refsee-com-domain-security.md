---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dns_aid:
    checked: '2026-11-22'
    published: false
  dnssec: false
  domain: refsee.com
  spf: true
hosts:
- cert_expires: Jan  7 19:30:08 2027 GMT
  host: refsee.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Refsee Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Refsee, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Refsee
provider_slug: refsee-com
slug: refsee-com-domain-security
source_filename: refsee-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-22'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: refsee.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  7 19:30:08 2027 GMT\n  hsts: false\ndomains:\n- domain: refsee.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n  dns_aid:\n    checked: '2026-11-22'\n    published: false\n"
source_yaml_url: https://artifacts.apis.io/refsee-com/security/refsee-com-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Video References
- AI Image
- AI Video
- AI Voices
- Moodboards
- Creative Pitch
- Search
- Portfolio
---
