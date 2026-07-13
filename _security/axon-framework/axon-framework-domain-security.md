---
api_specs:
- filename: axon-server-api.yml
  format: yaml
  label: Axon Framework
  slug: axon-framework
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/axon-framework/refs/heads/main/openapi/axon-server-api.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: axoniq.io
  spf: true
hosts:
- cert_expires: Aug 25 18:43:52 2026 GMT
  host: www.axoniq.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Axon Framework Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Axon Framework, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Axon Framework
provider_slug: axon-framework
slug: axon-framework-domain-security
source_filename: axon-framework-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.axoniq.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 25 18:43:52 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: axoniq.io\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/axon-framework/refs/heads/main/security/axon-framework-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- CQRS
- Event Sourcing
- Event-Driven
- Java
- Messaging
- Microservices
---
