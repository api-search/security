---
api_specs:
- filename: inflyu-com-public-api-openapi.yml
  format: yaml
  label: Inflyu Public API
  slug: inflyu-com-public-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/inflyu-com/openapi/inflyu-com-public-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 issue "amazon.com"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: inflyu.com
  spf: true
hosts:
- cert_expires: Dec 24 00:58:16 2026 GMT
  host: inflyu.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Inflyu Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Inflyu, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Inflyu
provider_slug: inflyu-com
slug: inflyu-com-domain-security
source_filename: inflyu-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: inflyu.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 24 00:58:16 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: inflyu.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/inflyu-com/security/inflyu-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Image Creation
- Audio Tools
- Influencer Tools
- Content Creation
---
