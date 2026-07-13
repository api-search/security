---
api_specs:
- filename: sportsdb-openapi.yml
  format: yaml
  label: TheSportsDB Search API
  slug: sportsdb-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sportsdb/refs/heads/main/openapi/sportsdb-openapi.yml
- filename: sportsdb-openapi.yml
  format: yaml
  label: TheSportsDB Lookups API
  slug: sportsdb-lookups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sportsdb/refs/heads/main/openapi/sportsdb-openapi.yml
- filename: sportsdb-openapi.yml
  format: yaml
  label: TheSportsDB Leagues API
  slug: sportsdb-leagues-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sportsdb/refs/heads/main/openapi/sportsdb-openapi.yml
- filename: sportsdb-openapi.yml
  format: yaml
  label: TheSportsDB Events & Schedules API
  slug: sportsdb-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sportsdb/refs/heads/main/openapi/sportsdb-openapi.yml
- filename: sportsdb-openapi.yml
  format: yaml
  label: TheSportsDB Livescores API
  slug: sportsdb-livescores-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sportsdb/refs/heads/main/openapi/sportsdb-openapi.yml
- filename: sportsdb-openapi.yml
  format: yaml
  label: TheSportsDB Players & Teams API
  slug: sportsdb-players-teams-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sportsdb/refs/heads/main/openapi/sportsdb-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: thesportsdb.com
  spf: true
hosts:
- cert_expires: Aug 21 01:45:09 2026 GMT
  host: www.thesportsdb.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Sportsdb Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for TheSportsDB, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: TheSportsDB
provider_slug: sportsdb
slug: sportsdb-domain-security
source_filename: sportsdb-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.thesportsdb.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 21 01:45:09 2026 GMT\n  hsts: false\ndomains:\n- domain: thesportsdb.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sportsdb/refs/heads/main/security/sportsdb-domain-security.yml
summary_line: TLSv1.3
tags:
- Sports
- Sports Data
- Teams
- Players
- Events
---
