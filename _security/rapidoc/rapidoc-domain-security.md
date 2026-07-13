---
api_specs:
- filename: rapidoc-rapidoc-openapi.yml
  format: yaml
  label: RapiDoc
  slug: rapidoc
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rapidoc/refs/heads/main/openapi/rapidoc-rapidoc-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: rapidocweb.com
  spf: true
hosts:
- cert_expires: Sep  5 03:53:04 2026 GMT
  host: rapidocweb.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Rapidoc Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for RapiDoc, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: RapiDoc
provider_slug: rapidoc
slug: rapidoc-domain-security
source_filename: rapidoc-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: rapidocweb.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  5 03:53:04 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: rapidocweb.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rapidoc/refs/heads/main/security/rapidoc-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Documentation
- Platform
- Web Components
- OpenAPI
---
