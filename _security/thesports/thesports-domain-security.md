---
api_specs:
- filename: thesports-football-openapi.yml
  format: yaml
  label: TheSports Football API
  slug: football-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thesports/refs/heads/main/openapi/thesports-football-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: thesports.com
  spf: true
hosts:
- cert_expires: Sep  5 04:08:52 2026 GMT
  host: www.thesports.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 15 23:18:17 2026 GMT
  host: api.thesports.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Thesports Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for TheSports, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: TheSports
provider_slug: thesports
slug: thesports-domain-security
source_filename: thesports-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.thesports.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  5 04:08:52 2026 GMT\n  hsts: false\n- host: api.thesports.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 23:18:17 2026 GMT\n  hsts: false\ndomains:\n- domain: thesports.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/thesports/refs/heads/main/security/thesports-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Sports
- Football
- Basketball
- Tennis
- Esports
- Data
- Real-Time
---
