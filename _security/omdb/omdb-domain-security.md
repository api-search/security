---
api_specs:
- filename: swagger.json
  format: json
  label: OMDb API
  slug: omdb-api
  spec_type: OpenAPI
  url: https://www.omdbapi.com/swagger.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: omdbapi.com
  spf: true
hosts:
- cert_expires: Aug 24 18:44:29 2026 GMT
  host: www.omdbapi.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 24 18:44:29 2026 GMT
  host: img.omdbapi.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Omdb Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for OMDb, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: OMDb
provider_slug: omdb
slug: omdb-domain-security
source_filename: omdb-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.omdbapi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 24 18:44:29 2026 GMT\n  hsts: false\n- host: img.omdbapi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 24 18:44:29 2026 GMT\n  hsts: false\ndomains:\n- domain: omdbapi.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/omdb/refs/heads/main/security/omdb-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Movies
- Television
- Entertainment
- Metadata
- Ratings
- Posters
- IMDb
- Open Data
---
