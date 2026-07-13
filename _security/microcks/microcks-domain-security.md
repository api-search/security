---
api_specs:
- filename: microcks-openapi.yml
  format: yaml
  label: Microcks API
  slug: microcks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microcks/refs/heads/main/openapi/microcks-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: microcks.io
  spf: false
hosts:
- cert_expires: Sep 21 23:32:22 2026 GMT
  host: microcks.io
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Microcks Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Microcks, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Microcks
provider_slug: microcks
slug: microcks-domain-security
source_filename: microcks-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: microcks.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 23:32:22 2026 GMT\n  hsts: false\ndomains:\n- domain: microcks.io\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/microcks/refs/heads/main/security/microcks-domain-security.yml
summary_line: TLSv1.3
tags:
- API Testing
- Cloud Native
- DevOps
- Mocking
- Open Source
---
