---
api_specs:
- filename: osisoft-pi-web-api-openapi.yml
  format: yaml
  label: OSIsoft PI Web API
  slug: pi-web-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/osisoft-pi/refs/heads/main/openapi/osisoft-pi-web-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: aveva.com
  spf: true
hosts:
- cert_expires: Sep 29 06:41:07 2026 GMT
  host: docs.aveva.com
  hsts: true
  hsts_max_age: 15638400
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 13 02:48:12 2026 GMT
  host: www.aveva.com
  hsts: true
  hsts_max_age: 15638400
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 24 23:59:59 2026 GMT
  host: api.aveva.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Osisoft Pi Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for osisoft-pi, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: osisoft-pi
provider_slug: osisoft-pi
slug: osisoft-pi-domain-security
source_filename: osisoft-pi-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: docs.aveva.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 06:41:07 2026 GMT\n  hsts: true\n  hsts_max_age: 15638400\n- host: www.aveva.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 13 02:48:12 2026 GMT\n  hsts: true\n  hsts_max_age: 15638400\n- host: api.aveva.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 24 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: aveva.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/osisoft-pi/refs/heads/main/security/osisoft-pi-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags: []
---
