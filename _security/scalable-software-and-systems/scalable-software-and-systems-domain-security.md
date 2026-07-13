---
api_specs:
- filename: scalable-software-and-systems-openapi.yml
  format: yaml
  label: Backstage Software Catalog API
  slug: backstage
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scalable-software-and-systems/refs/heads/main/openapi/scalable-software-and-systems-openapi.yml
- filename: openapi.yml
  format: yaml
  label: Temporal API
  slug: temporal
  spec_type: OpenAPI
  url: https://github.com/temporalio/api/blob/master/openapi/openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: backstage.io
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: cloudevents.io
  spf: false
hosts:
- cert_expires: Sep 27 15:01:52 2026 GMT
  host: backstage.io
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  3 01:48:35 2026 GMT
  host: cloudevents.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 24 23:33:10 2026 GMT
  host: kafka.apache.org
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Scalable Software And Systems Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Scalable Software and Systems, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Scalable Software and Systems
provider_slug: scalable-software-and-systems
slug: scalable-software-and-systems-domain-security
source_filename: scalable-software-and-systems-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: backstage.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 27 15:01:52 2026 GMT\n  hsts: false\n- host: cloudevents.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 01:48:35 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: kafka.apache.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 24 23:33:10 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: backstage.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n- domain: cloudevents.io\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/scalable-software-and-systems/refs/heads/main/security/scalable-software-and-systems-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- API First
- Architecture Patterns
- CQRS
- Distributed Systems
- Enterprise
- Event Driven
- Microservices
- Scalable Architecture
- Software Engineering
- Systems Design
---
