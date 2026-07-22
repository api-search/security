---
description: ''
domains:
- caa:
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 issue "amazon.com"
  - 0 issue "cloudflare.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: reqbin.com
  spf: true
hosts:
- cert_expires: Oct  9 15:41:10 2026 GMT
  host: reqbin.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Reqbin Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ReqBin, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: ReqBin
provider_slug: reqbin
slug: reqbin-domain-security
source_filename: reqbin-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: reqbin.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  9 15:41:10 2026 GMT\n  hsts: false\ndomains:\n- domain: reqbin.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"cloudflare.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/reqbin/refs/heads/main/security/reqbin-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- API Testing
- Browser
- Code Generation
- HTTP Client
- Online
---
