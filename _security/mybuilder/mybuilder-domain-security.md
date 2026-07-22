---
description: ''
domains:
- caa:
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "sectigo.com"
  - 0 issuewild "ssl.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: mybuilder.com
  spf: true
hosts:
- cert_expires: Sep  1 18:31:16 2026 GMT
  host: mybuilder.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Mybuilder Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for MyBuilder, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: MyBuilder
provider_slug: mybuilder
slug: mybuilder-domain-security
source_filename: mybuilder-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: mybuilder.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  1 18:31:16 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: mybuilder.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"sectigo.com\"\n  - 0 issuewild \"ssl.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mybuilder/refs/heads/main/security/mybuilder-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Home Services
- Marketplace
- Tradespeople
- Home Improvement
- Local Services
- United Kingdom
- Consumer
---
