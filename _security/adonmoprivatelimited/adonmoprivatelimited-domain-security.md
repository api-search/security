---
api_specs:
- filename: adonmoprivatelimited-adonmo-api.json
  format: json
  label: Adonmo API
  slug: adonmoprivatelimited-adonmo-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adonmoprivatelimited/refs/heads/main/openapi/adonmoprivatelimited-adonmo-api.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: adonmo.com
  spf: true
hosts:
- cert_expires: Dec  4 12:00:54 2026 GMT
  host: adonmo.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 27 13:01:29 2026 GMT
  host: api.adonmo.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: Adonmoprivatelimited Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Adonmo Private Limited, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Adonmo Private Limited
provider_slug: adonmoprivatelimited
slug: adonmoprivatelimited-domain-security
source_filename: adonmoprivatelimited-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-07'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: adonmo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  4 12:00:54 2026 GMT\n  hsts: false\n- host: api.adonmo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 27 13:01:29 2026 GMT\n  hsts: null\ndomains:\n- domain: adonmo.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/adonmoprivatelimited/refs/heads/main/security/adonmoprivatelimited-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Advertising
- Digital Out-of-Home
- DOOH
- Digital Signage
- AdTech
- Content Management
- Marketing
- India
- Company
---
