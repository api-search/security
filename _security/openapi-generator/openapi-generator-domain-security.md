---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: openapi-generator.tech
  spf: false
hosts:
- cert_expires: Sep 29 11:13:19 2026 GMT
  host: openapi-generator.tech
  hsts: true
  hsts_max_age: 31556952
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Openapi Generator Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for OpenAPI Generator, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: OpenAPI Generator
provider_slug: openapi-generator
slug: openapi-generator-domain-security
source_filename: openapi-generator-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: openapi-generator.tech\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 11:13:19 2026 GMT\n  hsts: true\n  hsts_max_age: 31556952\ndomains:\n- domain: openapi-generator.tech\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/openapi-generator/refs/heads/main/security/openapi-generator-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Code Generation
- Documentation
- Open Source
- OpenAPI
- SDK
---
