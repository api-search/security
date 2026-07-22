---
api_specs:
- filename: sequel-openapi-original.yml
  format: yaml
  label: Sequel (Introvoke) API
  slug: sequel-introvoke-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sequel/refs/heads/main/openapi/sequel-openapi-original.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: sequel.io
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: introvoke.com
  spf: true
hosts:
- cert_expires: Sep 21 14:50:13 2026 GMT
  host: sequel.io
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  8 23:59:59 2026 GMT
  host: api.introvoke.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Sequel Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Sequel, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Sequel
provider_slug: sequel
slug: sequel-domain-security
source_filename: sequel-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: sequel.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 14:50:13 2026 GMT\n  hsts: false\n- host: api.introvoke.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  8 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: sequel.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: introvoke.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sequel/refs/heads/main/security/sequel-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Webinars
- Virtual Events
- Live Streaming
- Video
- Networking
- Marketing
- Events
- Webhooks
---
