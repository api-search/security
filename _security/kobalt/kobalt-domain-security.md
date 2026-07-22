---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: kobaltmusic.com
  spf: true
hosts:
- cert_expires: Nov 20 23:59:59 2026 GMT
  host: kobaltmusic.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Kobalt Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Kobalt, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Kobalt
provider_slug: kobalt
slug: kobalt-domain-security
source_filename: kobalt-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: kobaltmusic.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 20 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: kobaltmusic.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kobalt/refs/heads/main/security/kobalt-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Music
- Music Publishing
- Rights Management
- Royalties
- Copyright
- Media and Entertainment
- Enterprise
---
