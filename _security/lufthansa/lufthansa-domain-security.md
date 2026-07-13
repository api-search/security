---
api_specs:
- filename: lufthansa-openapi.yml
  format: yaml
  label: Lufthansa Public API
  slug: public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lufthansa/refs/heads/main/openapi/lufthansa-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: lufthansagroup.com
  spf: false
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: lufthansa.com
  spf: true
hosts:
- cert_expires: Nov 14 23:59:59 2026 GMT
  host: www.lufthansagroup.com
  hsts: true
  hsts_max_age: 15768000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 30 23:59:59 2026 GMT
  host: developer.lufthansa.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 30 23:59:59 2026 GMT
  host: api.lufthansa.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Lufthansa Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Lufthansa, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF absent, DMARC present (p=reject).'
provider_name: Lufthansa
provider_slug: lufthansa
slug: lufthansa-domain-security
source_filename: lufthansa-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.lufthansagroup.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 14 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 15768000\n- host: developer.lufthansa.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 30 23:59:59 2026 GMT\n  hsts: false\n- host: api.lufthansa.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 30 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: lufthansagroup.com\n  dnssec: true\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: reject\n- domain: lufthansa.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lufthansa/refs/heads/main/security/lufthansa-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Airlines
- Travel
- Aviation
- Flights
---
