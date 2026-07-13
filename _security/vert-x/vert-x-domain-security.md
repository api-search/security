---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: vertx.io
  spf: false
hosts:
- cert_expires: Sep 12 12:28:47 2026 GMT
  host: vertx.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Vert X Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Vert.x, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Vert.x
provider_slug: vert-x
slug: vert-x-domain-security
source_filename: vert-x-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: vertx.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 12 12:28:47 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: vertx.io\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vert-x/refs/heads/main/security/vert-x-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Event-Driven
- Frameworks
- Java
- JVM
- Microservices
- Polyglot
- Reactive
- Eclipse Foundation
- Open Source
---
