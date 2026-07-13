---
api_specs:
- filename: growthbook-openapi.yaml
  format: yaml
  label: GrowthBook REST API
  slug: growthbook-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/growthbook/refs/heads/main/openapi/growthbook-openapi.yaml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: growthbook.io
  spf: true
hosts:
- cert_expires: Sep 24 12:14:47 2026 GMT
  host: www.growthbook.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 17 02:34:31 2026 GMT
  host: docs.growthbook.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 30 23:59:59 2026 GMT
  host: api.growthbook.io
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Growthbook Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for GrowthBook, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: GrowthBook
provider_slug: growthbook
slug: growthbook-domain-security
source_filename: growthbook-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.growthbook.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 12:14:47 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.growthbook.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 17 02:34:31 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.growthbook.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 30 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: growthbook.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/growthbook/refs/heads/main/security/growthbook-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Feature Flags
- Experimentation
- Open Source
- AB Testing
- Analytics
---
