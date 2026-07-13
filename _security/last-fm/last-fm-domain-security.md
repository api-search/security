---
api_specs:
- filename: last-fm-openapi.yml
  format: yaml
  label: Last.fm API
  slug: last-fm-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/last-fm/refs/heads/main/openapi/last-fm-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: last.fm
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: audioscrobbler.com
  spf: true
hosts:
- cert_expires: Mar 25 23:59:59 2027 GMT
  host: www.last.fm
  hsts: true
  hsts_max_age: 300
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 10 23:59:59 2026 GMT
  host: ws.audioscrobbler.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Last Fm Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Last.fm, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Last.fm
provider_slug: last-fm
slug: last-fm-domain-security
source_filename: last-fm-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.last.fm\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 25 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 300\n- host: ws.audioscrobbler.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 10 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: last.fm\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: audioscrobbler.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/last-fm/refs/heads/main/security/last-fm-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Music
- Music Metadata
- Scrobbling
- Music Discovery
- Streaming
---
