---
api_specs:
- filename: architecture-pattern-domains-api-openapi.yml
  format: yaml
  label: Architecture Pattern Domains API
  slug: architecture-pattern-domains-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/architecture-pattern/refs/heads/main/openapi/architecture-pattern-domains-api-openapi.yml
- filename: architecture-pattern-patterns-api-openapi.yml
  format: yaml
  label: Architecture Pattern Patterns API
  slug: architecture-pattern-patterns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/architecture-pattern/refs/heads/main/openapi/architecture-pattern-patterns-api-openapi.yml
- filename: architecture-pattern-trade-offs-api-openapi.yml
  format: yaml
  label: Architecture Pattern Trade-offs API
  slug: architecture-pattern-trade-offs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/architecture-pattern/refs/heads/main/openapi/architecture-pattern-trade-offs-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: microservices.io
  spf: true
hosts:
- cert_expires: Sep 30 00:31:22 2026 GMT
  host: microservices.io
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Architecture Pattern Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Architecture Pattern, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Architecture Pattern
provider_slug: architecture-pattern
slug: architecture-pattern-domain-security
source_filename: architecture-pattern-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: microservices.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 00:31:22 2026 GMT\n  hsts: false\ndomains:\n- domain: microservices.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/architecture-pattern/refs/heads/main/security/architecture-pattern-domain-security.yml
summary_line: TLSv1.3
tags:
- Architecture Patterns
- Software Architecture
- Design Patterns
- System Design
- Microservices
- Cloud Native
---
