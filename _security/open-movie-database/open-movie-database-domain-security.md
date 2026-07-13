---
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
kind: domain-security
layout: security
method: probed
name: Open Movie Database Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Open Movie Database, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Open Movie Database
provider_slug: open-movie-database
slug: open-movie-database-domain-security
source_filename: open-movie-database-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.omdbapi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 24 18:44:29 2026 GMT\n  hsts: false\ndomains:\n- domain: omdbapi.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/open-movie-database/refs/heads/main/security/open-movie-database-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Video
- Public APIs
---
