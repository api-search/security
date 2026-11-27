---
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "sectigo.com"
  - 0 issue "ssl.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: simpleverifier.com
  spf: true
hosts:
- cert_expires: Jan 19 21:44:37 2027 GMT
  host: simpleverifier.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: SimpleVerifier Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SimpleVerifier, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: SimpleVerifier
provider_slug: simpleverifier-com
slug: simpleverifier-com-domain-security
source_filename: simpleverifier-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: simpleverifier.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 19 21:44:37 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: simpleverifier.com\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/simpleverifier-com/security/simpleverifier-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Email Verification
- Software-as-a-Service
- Bulk Tools
- Security
---
