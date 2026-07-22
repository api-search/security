---
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
name: Restful Microservices Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for RESTful Microservices, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: RESTful Microservices
provider_slug: restful-microservices
slug: restful-microservices-domain-security
source_filename: restful-microservices-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: microservices.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 00:31:22 2026 GMT\n  hsts: false\ndomains:\n- domain: microservices.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/restful-microservices/refs/heads/main/security/restful-microservices-domain-security.yml
summary_line: TLSv1.3
tags:
- Architecture
- Distributed Systems
- Microservices
- REST
- Kubernetes
- Service Mesh
- Cloud Native
---
