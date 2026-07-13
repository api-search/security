---
description: ''
domains:
- caa:
  - 0 issue "amazonaws.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "sectigo.com"
  dmarc: false
  dnssec: false
  domain: gitter.im
  spf: true
hosts:
- host: developer.gitter.im
  https: false
kind: domain-security
layout: security
method: probed
name: Gitter Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Gitter, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Gitter
provider_slug: gitter
slug: gitter-domain-security
source_filename: gitter-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developer.gitter.im\n  https: false\ndomains:\n- domain: gitter.im\n  dnssec: false\n  caa:\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"sectigo.com\"\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gitter/refs/heads/main/security/gitter-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Development
- Public APIs
---
