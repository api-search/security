---
api_specs:
- filename: 3.0.0
  format: yaml
  label: Bandsintown Public API
  slug: public-api
  spec_type: OpenAPI
  url: https://app.swaggerhub.com/apis/Bandsintown/PublicAPI/3.0.0
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: bandsintown.com
  spf: true
hosts:
- cert_expires: Aug 12 17:58:07 2026 GMT
  host: www.bandsintown.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan  7 23:59:59 2027 GMT
  host: help.artists.bandsintown.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan  5 23:59:59 2027 GMT
  host: rest.bandsintown.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Bandsintown Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bandsintown, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Bandsintown
provider_slug: bandsintown
slug: bandsintown-domain-security
source_filename: bandsintown-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.bandsintown.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 12 17:58:07 2026 GMT\n  hsts: null\n- host: help.artists.bandsintown.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  7 23:59:59 2027 GMT\n  hsts: false\n- host: rest.bandsintown.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  5 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: bandsintown.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bandsintown/refs/heads/main/security/bandsintown-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- concerts
- live music
- events
- artists
- venues
- music discovery
- tour dates
- tickets
- fan notifications
- entertainment
---
