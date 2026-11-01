---
description: ''
domains:
- caa:
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  - 0 issuewild "amazon.com"
  - 0 issuewild "amazontrust.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: insanejournal.com
  spf: true
hosts:
- cert_expires: Dec 15 03:15:13 2026 GMT
  host: insanejournal.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Insanejournal Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for InsaneJournal, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: InsaneJournal
provider_slug: insanejournal
slug: insanejournal-domain-security
source_filename: insanejournal-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: insanejournal.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 15 03:15:13 2026 GMT\n  hsts: null\ndomains:\n- domain: insanejournal.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"amazon.com\"\n  - 0 issuewild \"amazontrust.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/insanejournal/security/insanejournal-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Blogging
- Journaling
- Social Networking
- Online Communities
- LiveJournal Codebase
---
