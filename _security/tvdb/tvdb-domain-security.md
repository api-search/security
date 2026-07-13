---
api_specs:
- filename: tvdb-openapi.yml
  format: yaml
  label: TheTVDB v4 API
  slug: tvdb-v4-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tvdb/refs/heads/main/openapi/tvdb-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: thetvdb.com
  spf: true
hosts:
- cert_expires: Jan 21 23:59:59 2027 GMT
  host: thetvdb.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 21 23:59:59 2027 GMT
  host: api4.thetvdb.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Tvdb Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for TheTVDB, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: TheTVDB
provider_slug: tvdb
slug: tvdb-domain-security
source_filename: tvdb-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: thetvdb.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 21 23:59:59 2027 GMT\n  hsts: false\n- host: api4.thetvdb.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 21 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: thetvdb.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tvdb/refs/heads/main/security/tvdb-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Entertainment
- Movies
- Television
- Media Metadata
- Public APIs
- Video
---
