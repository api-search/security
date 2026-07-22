---
api_specs:
- filename: sleeper-openapi.yml
  format: yaml
  label: Sleeper API
  slug: sleeper-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sleeper/refs/heads/main/openapi/sleeper-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: sleeper.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: sleeper.app
  spf: true
hosts:
- cert_expires: Sep 20 14:05:19 2026 GMT
  host: docs.sleeper.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 21 21:44:25 2026 GMT
  host: api.sleeper.app
  hsts: true
  hsts_max_age: 15724800
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Sleeper Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Sleeper, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Sleeper
provider_slug: sleeper
slug: sleeper-domain-security
source_filename: sleeper-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: docs.sleeper.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 14:05:19 2026 GMT\n  hsts: false\n- host: api.sleeper.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 21:44:25 2026 GMT\n  hsts: true\n  hsts_max_age: 15724800\ndomains:\n- domain: sleeper.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: sleeper.app\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sleeper/refs/heads/main/security/sleeper-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Fantasy Sports
- Sports
- Fantasy Football
- Gaming
- Sports Data
- Leagues
- Consumer
---
