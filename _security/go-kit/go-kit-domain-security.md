---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: gokit.io
  spf: false
hosts:
- cert_expires: Sep 26 23:43:54 2026 GMT
  host: gokit.io
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Go Kit Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Go Kit, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Go Kit
provider_slug: go-kit
slug: go-kit-domain-security
source_filename: go-kit-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: gokit.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 23:43:54 2026 GMT\n  hsts: false\ndomains:\n- domain: gokit.io\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/go-kit/refs/heads/main/security/go-kit-domain-security.yml
summary_line: TLSv1.3
tags:
- Distributed Systems
- Domain-Driven Design
- Frameworks
- Go
- Golang
- Microservices
---
