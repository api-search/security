---
description: ''
domains:
- caa:
  - 0 issuewild "amazon.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "globalsign.com"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: digite.com
  spf: true
hosts:
- cert_expires: Aug 28 11:54:11 2026 GMT
  host: www.digite.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Swiftkanban Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SwiftKanban, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: SwiftKanban
provider_slug: swiftkanban
slug: swiftkanban-domain-security
source_filename: swiftkanban-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.digite.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 28 11:54:11 2026 GMT\n  hsts: null\ndomains:\n- domain: digite.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"amazon.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"globalsign.com\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/swiftkanban/refs/heads/main/security/swiftkanban-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Business
- Public APIs
---
