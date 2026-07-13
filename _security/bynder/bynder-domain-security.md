---
api_specs:
- filename: bynder-openapi.yml
  format: yaml
  label: Bynder API
  slug: bynder-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bynder/refs/heads/main/openapi/bynder-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: bynder.com
  spf: true
hosts:
- cert_expires: Aug 12 16:12:31 2026 GMT
  host: www.bynder.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 29 17:57:25 2026 GMT
  host: developers.bynder.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- host: yourportal.bynder.com
  https: false
kind: domain-security
layout: security
method: probed
name: Bynder Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bynder, probed live across 3 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Bynder
provider_slug: bynder
slug: bynder-domain-security
source_filename: bynder-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.bynder.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 12 16:12:31 2026 GMT\n  hsts: null\n- host: developers.bynder.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 17:57:25 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: yourportal.bynder.com\n  https: false\ndomains:\n- domain: bynder.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bynder/refs/heads/main/security/bynder-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Digital Asset Management
- DAM
- Brand Management
- Content Management
- Marketing
---
