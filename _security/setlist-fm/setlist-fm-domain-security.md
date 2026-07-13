---
api_specs:
- filename: swagger.json
  format: json
  label: setlist.fm API
  slug: setlist-fm-api
  spec_type: OpenAPI
  url: https://api.setlist.fm/docs/1.0/ui/swagger.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: setlist.fm
  spf: true
hosts:
- cert_expires: Dec  8 23:59:59 2026 GMT
  host: www.setlist.fm
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  8 23:59:59 2026 GMT
  host: api.setlist.fm
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Setlist Fm Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for setlist.fm, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: setlist.fm
provider_slug: setlist-fm
slug: setlist-fm-domain-security
source_filename: setlist-fm-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.setlist.fm\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  8 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.setlist.fm\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  8 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: setlist.fm\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/setlist-fm/refs/heads/main/security/setlist-fm-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Music
- Concerts
- Setlists
- Live Music
- Venues
- Artists
- Tour Dates
- Events
---
