---
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
  dmarc_policy: none
  dnssec: false
  domain: sameerkumar.website
  spf: true
hosts:
- cert_expires: Aug 29 17:18:13 2026 GMT
  host: aztro.sameerkumar.website
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Aztro Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for aztro, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: aztro
provider_slug: aztro
slug: aztro-domain-security
source_filename: aztro-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: aztro.sameerkumar.website\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 29 17:18:13 2026 GMT\n  hsts: null\ndomains:\n- domain: sameerkumar.website\n  dnssec: false\n  caa:\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aztro/refs/heads/main/security/aztro-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Social
- Public APIs
---
