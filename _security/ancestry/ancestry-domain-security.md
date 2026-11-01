---
description: ''
domains:
- caa:
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "thawte.com"
  - 0 issue "amazon.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com"
  - 0 issue "globalsign.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: ancestry.com
  spf: true
hosts:
- cert_expires: Dec  1 05:26:54 2026 GMT
  host: ancestry.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Ancestry Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ancestry TreeShare download + WebHints, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Ancestry TreeShare download + WebHints
provider_slug: ancestry
slug: ancestry-domain-security
source_filename: ancestry-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ancestry.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  1 05:26:54 2026 GMT\n  hsts: null\ndomains:\n- domain: ancestry.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"thawte.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"globalsign.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/ancestry/security/ancestry-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Genealogy
- DataExport
- WebTools
- FamilyHistory
---
