---
api_specs:
- filename: asyncapi.md
  format: yaml
  label: AsyncAPI Specification
  slug: asyncapi-spec
  spec_type: AsyncAPI
  url: https://github.com/asyncapi/spec/blob/master/spec/asyncapi.md
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: asyncapi.com
  spf: false
hosts:
- cert_expires: Oct  1 03:28:50 2026 GMT
  host: www.asyncapi.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Asyncapi Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AsyncAPI, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: AsyncAPI
provider_slug: asyncapi
slug: asyncapi-domain-security
source_filename: asyncapi-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.asyncapi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 03:28:50 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: asyncapi.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/asyncapi/refs/heads/main/security/asyncapi-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Event-Driven
- Linux Foundation
- Messaging
- Standards
- Specification
---
