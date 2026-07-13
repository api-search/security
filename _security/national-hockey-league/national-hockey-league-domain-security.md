---
api_specs:
- filename: national-hockey-league-openapi.yml
  format: yaml
  label: NHL Web API
  slug: nhl-web-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/national-hockey-league/refs/heads/main/openapi/national-hockey-league-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: nhl.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: nhle.com
  spf: true
hosts:
- cert_expires: Sep 11 08:57:00 2026 GMT
  host: www.nhl.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 26 04:30:44 2026 GMT
  host: api-web.nhle.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 26 04:30:44 2026 GMT
  host: api.nhle.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: National Hockey League Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for National Hockey League, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: National Hockey League
provider_slug: national-hockey-league
slug: national-hockey-league-domain-security
source_filename: national-hockey-league-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.nhl.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 11 08:57:00 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api-web.nhle.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 04:30:44 2026 GMT\n  hsts: null\n- host: api.nhle.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 04:30:44 2026 GMT\n  hsts: null\ndomains:\n- domain: nhl.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: nhle.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/national-hockey-league/refs/heads/main/security/national-hockey-league-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Sports
- Hockey
- Entertainment
- Professional League
---
