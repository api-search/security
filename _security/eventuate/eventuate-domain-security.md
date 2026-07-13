---
api_specs:
- filename: eventuate-api.yml
  format: yaml
  label: Eventuate
  slug: eventuate
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eventuate/refs/heads/main/openapi/eventuate-api.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: eventuate.io
  spf: false
hosts:
- cert_expires: Sep 24 17:26:52 2026 GMT
  host: eventuate.io
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Eventuate Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Eventuate, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Eventuate
provider_slug: eventuate
slug: eventuate-domain-security
source_filename: eventuate-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: eventuate.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 17:26:52 2026 GMT\n  hsts: false\ndomains:\n- domain: eventuate.io\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/eventuate/refs/heads/main/security/eventuate-domain-security.yml
summary_line: TLSv1.3
tags:
- CQRS
- Distributed Data
- Event Sourcing
- Event-Driven
- Microservices
- Sagas
---
