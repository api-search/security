---
api_specs:
- filename: thegamesdb-openapi.yml
  format: yaml
  label: TheGamesDB API
  slug: thegamesdb
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thegamesdb/refs/heads/main/openapi/thegamesdb-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: thegamesdb.net
  spf: true
hosts:
- cert_expires: Sep 16 21:15:06 2026 GMT
  host: thegamesdb.net
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 15 16:15:20 2026 GMT
  host: api.thegamesdb.net
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Thegamesdb Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for TheGamesDB, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: TheGamesDB
provider_slug: thegamesdb
slug: thegamesdb-domain-security
source_filename: thegamesdb-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: thegamesdb.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 21:15:06 2026 GMT\n  hsts: false\n- host: api.thegamesdb.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 16:15:20 2026 GMT\n  hsts: false\ndomains:\n- domain: thegamesdb.net\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/thegamesdb/refs/heads/main/security/thegamesdb-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Database
- Gaming
- Video Games
- Metadata
- Artwork
---
