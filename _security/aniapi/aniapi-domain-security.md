---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: aniapi.com
  spf: false
hosts:
- cert_expires: Aug 23 05:54:06 2026 GMT
  host: aniapi.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Aniapi Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AniAPI, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: AniAPI
provider_slug: aniapi
slug: aniapi-domain-security
source_filename: aniapi-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: aniapi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 23 05:54:06 2026 GMT\n  hsts: null\ndomains:\n- domain: aniapi.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aniapi/refs/heads/main/security/aniapi-domain-security.yml
summary_line: TLSv1.3
tags:
- Anime
- Public APIs
---
