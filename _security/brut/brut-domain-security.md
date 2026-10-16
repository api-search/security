---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: brut.media
  spf: true
hosts:
- cert_expires: Nov 27 16:47:55 2026 GMT
  host: brands.brut.media
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Brut Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Brut, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Brut
provider_slug: brut
slug: brut-domain-security
source_filename: brut-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-06'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: brands.brut.media\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 27 16:47:55 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: brut.media\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/brut/refs/heads/main/security/brut-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Media
- News
- Social
- Video
- Advertising
---
