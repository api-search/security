---
description: ''
domains:
- caa:
  - 0 contactemail "caarecordaware@microsoft.com"
  - 0 iodef "mailto:caarecordaware@microsoft.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: typespec.io
  spf: false
hosts:
- cert_expires: Oct  7 11:50:18 2026 GMT
  host: typespec.io
  hsts: true
  hsts_max_age: 31556952
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Typespec Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for TypeSpec, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=reject).'
provider_name: TypeSpec
provider_slug: typespec
slug: typespec-domain-security
source_filename: typespec-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: typespec.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 11:50:18 2026 GMT\n  hsts: true\n  hsts_max_age: 31556952\ndomains:\n- domain: typespec.io\n  dnssec: false\n  caa:\n  - 0 contactemail \"caarecordaware@microsoft.com\"\n  - 0 iodef \"mailto:caarecordaware@microsoft.com\"\n  spf: false\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/typespec/refs/heads/main/security/typespec-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- API Design
- Code Generation
- OpenAPI
- Protocol Buffers
- Specification Language
---
