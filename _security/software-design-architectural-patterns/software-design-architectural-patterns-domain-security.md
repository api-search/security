---
description: ''
domains:
- caa:
  - 0 contactemail "caarecordaware@microsoft.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: microsoft.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: microservices.io
  spf: true
hosts:
- cert_expires: Dec 11 02:26:09 2026 GMT
  host: learn.microsoft.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 30 00:31:22 2026 GMT
  host: microservices.io
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Software Design Architectural Patterns Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Software Design Architectural Patterns, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Software Design Architectural Patterns
provider_slug: software-design-architectural-patterns
slug: software-design-architectural-patterns-domain-security
source_filename: software-design-architectural-patterns-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: learn.microsoft.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 11 02:26:09 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: microservices.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 00:31:22 2026 GMT\n  hsts: false\ndomains:\n- domain: microsoft.com\n  dnssec: false\n  caa:\n  - 0 contactemail \"caarecordaware@microsoft.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: microservices.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/software-design-architectural-patterns/refs/heads/main/security/software-design-architectural-patterns-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Best Practices
- Design Patterns
- Software Architecture
- System Design
- Microservices
- MVC
- CQRS
- Event-Driven
---
