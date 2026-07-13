---
api_specs:
- filename: akka-management.json
  format: json
  label: Akka Management
  slug: akka-management
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/akka/refs/heads/main/openapi/akka-management.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: akka.io
  spf: true
hosts:
- cert_expires: Sep 25 12:01:53 2026 GMT
  host: akka.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  1 15:03:40 2026 GMT
  host: doc.akka.io
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Akka Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Akka, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Akka
provider_slug: akka
slug: akka-domain-security
source_filename: akka-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: akka.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 12:01:53 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: doc.akka.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  1 15:03:40 2026 GMT\n  hsts: false\ndomains:\n- domain: akka.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/akka/refs/heads/main/security/akka-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Actor Model
- Distributed Systems
- Frameworks
- Java
- Microservices
- Reactive
- Scala
---
