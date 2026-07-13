---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: go-micro.dev
  spf: true
hosts:
- cert_expires: Aug 17 16:39:30 2026 GMT
  host: go-micro.dev
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Go Micro Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Go Micro, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Go Micro
provider_slug: go-micro
slug: go-micro-domain-security
source_filename: go-micro-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: go-micro.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 17 16:39:30 2026 GMT\n  hsts: false\ndomains:\n- domain: go-micro.dev\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/go-micro/refs/heads/main/security/go-micro-domain-security.yml
summary_line: TLSv1.3
tags:
- Distributed Systems
- Frameworks
- Go
- Golang
- Microservices
- RPC
- Service Discovery
---
