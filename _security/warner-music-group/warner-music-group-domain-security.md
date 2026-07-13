---
api_specs:
- filename: warner-music-group-licensing-openapi.yml
  format: yaml
  label: Warner Music Group Licensing API
  slug: wmg-licensing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/warner-music-group/refs/heads/main/openapi/warner-music-group-licensing-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: wmg.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: wmgmusiclicensing.com
  spf: true
hosts:
- cert_expires: Sep 17 03:18:46 2026 GMT
  host: www.wmg.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 15 23:59:59 2027 GMT
  host: www.wmgmusiclicensing.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  3 09:55:47 2026 GMT
  host: warnerchappell.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Warner Music Group Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Warner Music Group, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Warner Music Group
provider_slug: warner-music-group
slug: warner-music-group-domain-security
source_filename: warner-music-group-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.wmg.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 17 03:18:46 2026 GMT\n  hsts: false\n- host: www.wmgmusiclicensing.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 15 23:59:59 2027 GMT\n  hsts: false\n- host: warnerchappell.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  3 09:55:47 2026 GMT\n  hsts: false\ndomains:\n- domain: wmg.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: wmgmusiclicensing.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/warner-music-group/refs/heads/main/security/warner-music-group-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Music
- Entertainment
- Streaming
- Licensing
- Publishing
---
