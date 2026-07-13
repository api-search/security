---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: freeforexapi.com
  spf: false
hosts:
- cert_expires: Oct  3 18:04:59 2026 GMT
  host: freeforexapi.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Freeforexapi Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for FreeForexAPI, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: FreeForexAPI
provider_slug: freeforexapi
slug: freeforexapi-domain-security
source_filename: freeforexapi-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: freeforexapi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 18:04:59 2026 GMT\n  hsts: null\ndomains:\n- domain: freeforexapi.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/freeforexapi/refs/heads/main/security/freeforexapi-domain-security.yml
summary_line: TLSv1.3
tags:
- Currency Exchange
- Public APIs
---
