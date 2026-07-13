---
description: ''
domains:
- caa:
  - 0 issuewild "www.digicert.com"
  - 0 issuewild "digicert.com"
  - 0 issuewild "godaddy.com"
  - 0 issuewild "pki.goog"
  - 0 issuewild "sectigo.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: btcturk.com
  spf: true
hosts:
- cert_expires: Aug 29 01:19:23 2026 GMT
  host: docs.btcturk.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Btcturk Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for BtcTurk, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: BtcTurk
provider_slug: btcturk
slug: btcturk-domain-security
source_filename: btcturk-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: docs.btcturk.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 29 01:19:23 2026 GMT\n  hsts: false\ndomains:\n- domain: btcturk.com\n  dnssec: true\n  caa:\n  - 0 issuewild \"www.digicert.com\"\n  - 0 issuewild \"digicert.com\"\n  - 0 issuewild \"godaddy.com\"\n  - 0 issuewild \"pki.goog\"\n  - 0 issuewild \"sectigo.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/btcturk/refs/heads/main/security/btcturk-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Cryptocurrency
- Public APIs
---
