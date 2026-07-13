---
api_specs:
- filename: matrix-openapi.yml
  format: yaml
  label: Matrix Client-Server API
  slug: client-server-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/matrix/refs/heads/main/openapi/matrix-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "amazontrust.com"
  - 0 issuewild "awstrust.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: matrix.org
  spf: true
hosts:
- cert_expires: Sep 10 12:59:13 2026 GMT
  host: matrix.org
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  6 19:46:11 2026 GMT
  host: spec.matrix.org
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Matrix Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Matrix, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Matrix
provider_slug: matrix
slug: matrix-domain-security
source_filename: matrix-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: matrix.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 10 12:59:13 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: spec.matrix.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 19:46:11 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: matrix.org\n  dnssec: false\n  caa:\n  - 0 issuewild \"amazontrust.com\"\n  - 0 issuewild \"awstrust.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/matrix/refs/heads/main/security/matrix-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Messaging
- Decentralized
- Federated
- Open Standard
- Real-Time Communication
- VoIP
---
