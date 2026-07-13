---
api_specs:
- filename: hp-workforce-solutions-analytics-api-openapi.yml
  format: yaml
  label: HP Workforce Solutions Analytics API
  slug: hp-workforce-solutions-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hp/refs/heads/main/openapi/hp-workforce-solutions-analytics-api-openapi.yml
- filename: hp-printos-device-api-openapi.yml
  format: yaml
  label: HP PrintOS Device API
  slug: hp-printos-device-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hp/refs/heads/main/openapi/hp-printos-device-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: hp.com
  spf: true
hosts:
- cert_expires: Oct 21 23:59:59 2026 GMT
  host: www.hp.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  7 23:59:59 2026 GMT
  host: developers.hp.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 24 23:59:59 2026 GMT
  host: daas.api.hp.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Hp Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for HP, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: HP
provider_slug: hp
slug: hp-domain-security
source_filename: hp-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.hp.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 21 23:59:59 2026 GMT\n  hsts: null\n- host: developers.hp.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 23:59:59 2026 GMT\n  hsts: null\n- host: daas.api.hp.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Aug 24 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: hp.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hp/refs/heads/main/security/hp-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Computer Hardware
- Device Management
- Printing
- Technology
- Fortune 100
---
