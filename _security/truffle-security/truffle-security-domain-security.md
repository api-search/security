---
description: ''
domains:
- caa:
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 issue "comodoca.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: trufflesecurity.com
  spf: true
hosts:
- cert_expires: Sep 28 12:44:29 2026 GMT
  host: trufflesecurity.com
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 28 12:44:29 2026 GMT
  host: docs.trufflesecurity.com
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Truffle Security Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Truffle Security, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Truffle Security
provider_slug: truffle-security
slug: truffle-security-domain-security
source_filename: truffle-security-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: trufflesecurity.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 12:44:29 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\n- host: docs.trufflesecurity.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 12:44:29 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\ndomains:\n- domain: trufflesecurity.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"comodoca.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/truffle-security/refs/heads/main/security/truffle-security-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Security
- Secrets Detection
- Secrets Scanning
- DevSecOps
- Application Security
- Credential Scanning
- TruffleHog
- Open-Source
---
