---
api_specs:
- filename: socket-openapi-original.json
  format: json
  label: Socket API
  slug: socket-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/socket/refs/heads/main/openapi/socket-openapi-original.json
description: ''
domains:
- caa:
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  - 0 issuewild "comodoca.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: socket.dev
  spf: true
hosts:
- cert_expires: Oct 13 20:25:39 2026 GMT
  host: socket.dev
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  7 00:20:47 2026 GMT
  host: docs.socket.dev
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 13 20:12:14 2026 GMT
  host: api.socket.dev
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Socket Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Socket, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Socket
provider_slug: socket
slug: socket-domain-security
source_filename: socket-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: socket.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 13 20:25:39 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.socket.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  7 00:20:47 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.socket.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 13 20:12:14 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: socket.dev\n  dnssec: true\n  caa:\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/socket/refs/heads/main/security/socket-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Security
- Software Supply Chain Security
- Dependency Scanning
- Software Composition Analysis
- Vulnerability Management
- Open Source Security
- DevSecOps
- SBOM
- Package Analysis
---
