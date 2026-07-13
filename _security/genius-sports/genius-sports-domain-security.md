---
api_specs:
- filename: swagger-latest.json
  format: json
  label: Genius Sports Fixtures API v2
  slug: fixtures-api-v2
  spec_type: OpenAPI
  url: https://explorer.api.geniussports.com/Fixtures/v2/Production/swagger-latest.json
- filename: swagger-latest.json
  format: json
  label: Genius Sports Matching API v2
  slug: matching-api-v2
  spec_type: OpenAPI
  url: https://explorer.api.geniussports.com/fixtures-matching/v2/Production/swagger-latest.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: geniussports.com
  spf: true
hosts:
- cert_expires: Jan  5 23:59:59 2027 GMT
  host: geniussports.com
  hsts: true
  hsts_max_age: 86400
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 12 23:59:59 2027 GMT
  host: developer.geniussports.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 22 23:59:59 2027 GMT
  host: fixtures.api.geniussports.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Genius Sports Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Genius Sports, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Genius Sports
provider_slug: genius-sports
slug: genius-sports-domain-security
source_filename: genius-sports-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: geniussports.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  5 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 86400\n- host: developer.geniussports.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 12 23:59:59 2027 GMT\n  hsts: false\n- host: fixtures.api.geniussports.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 22 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: geniussports.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/genius-sports/refs/heads/main/security/genius-sports-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Sports
- Statistics
- Live Data
- Fixtures
---
