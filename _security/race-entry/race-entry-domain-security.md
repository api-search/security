---
api_specs:
- filename: race-entry-openapi.yml
  format: yaml
  label: Race Entry
  slug: race-entry
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/race-entry/refs/heads/main/openapi/race-entry-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: raceentry.com
  spf: true
hosts:
- cert_expires: Sep 17 23:59:59 2026 GMT
  host: www.raceentry.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 15 14:24:00 2026 GMT
  host: demo.raceentry.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Race Entry Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Race Entry, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Race Entry
provider_slug: race-entry
slug: race-entry-domain-security
source_filename: race-entry-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.raceentry.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 17 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: demo.raceentry.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 15 14:24:00 2026 GMT\n  hsts: false\ndomains:\n- domain: raceentry.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/race-entry/refs/heads/main/security/race-entry-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Race Timing
- Race Registration
- Event Management
- Race Results
- Sports
---
