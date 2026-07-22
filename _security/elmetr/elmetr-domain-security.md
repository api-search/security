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
  dmarc: false
  dnssec: false
  domain: elmetr.com
  spf: true
hosts:
- cert_expires: Oct  4 14:28:25 2026 GMT
  host: elmetr.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Elmetr Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ElMetr, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: ElMetr
provider_slug: elmetr
slug: elmetr-domain-security
source_filename: elmetr-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: elmetr.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 14:28:25 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: elmetr.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"comodoca.com\"\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/elmetr/refs/heads/main/security/elmetr-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Legal
- Legal Services
- Legal Tech
- Legal Consultation
- Compliance
- Startups
- Saudi Arabia
- Egypt
- Middle East
---
