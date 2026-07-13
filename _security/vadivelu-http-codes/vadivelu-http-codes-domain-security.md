---
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: anoram.com
  spf: true
hosts:
- host: vadivelu.anoram.com
  https: false
kind: domain-security
layout: security
method: probed
name: Vadivelu Http Codes Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Vadivelu HTTP Codes, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Vadivelu HTTP Codes
provider_slug: vadivelu-http-codes
slug: vadivelu-http-codes-domain-security
source_filename: vadivelu-http-codes-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: vadivelu.anoram.com\n  https: false\ndomains:\n- domain: anoram.com\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vadivelu-http-codes/refs/heads/main/security/vadivelu-http-codes-domain-security.yml
summary_line: DMARC
tags:
- Personality
- Public APIs
---
