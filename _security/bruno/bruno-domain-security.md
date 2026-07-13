---
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  - 0 issuewild "amazonaws.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: usebruno.com
  spf: true
hosts:
- cert_expires: Jan 21 23:59:59 2027 GMT
  host: www.usebruno.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Bruno Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bruno, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Bruno
provider_slug: bruno
slug: bruno-domain-security
source_filename: bruno-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.usebruno.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan 21 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: usebruno.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  - 0 issuewild \"amazonaws.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bruno/refs/heads/main/security/bruno-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- API Client
- API Testing
- CLI
- Git
- GraphQL
- gRPC
- JavaScript
- MIT License
- Open Source
- REST
---
