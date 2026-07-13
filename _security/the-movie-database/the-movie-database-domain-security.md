---
api_specs:
- filename: tmdb-api.json
  format: json
  label: The Movie Database API
  slug: the-movie-database
  spec_type: OpenAPI
  url: https://developer.themoviedb.org/openapi/tmdb-api.json
description: ''
domains:
- caa:
  - 0 issue "comodoca.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "awstrust.com"
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: themoviedb.org
  spf: true
hosts:
- cert_expires: Dec  2 23:59:59 2026 GMT
  host: www.themoviedb.org
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 28 20:55:03 2026 GMT
  host: developer.themoviedb.org
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  2 23:59:59 2026 GMT
  host: api.themoviedb.org
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: The Movie Database Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for The Movie Database, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: The Movie Database
provider_slug: the-movie-database
slug: the-movie-database-domain-security
source_filename: the-movie-database-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.themoviedb.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  2 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.themoviedb.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 20:55:03 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.themoviedb.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  2 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: themoviedb.org\n  dnssec: true\n  caa:\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"awstrust.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/the-movie-database/refs/heads/main/security/the-movie-database-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Entertainment
- Movies
- Television
---
