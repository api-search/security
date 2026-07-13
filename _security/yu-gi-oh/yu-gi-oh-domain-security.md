---
api_specs:
- filename: yu-gi-oh-ygoprodeck-openapi.yml
  format: yaml
  label: YGOPRODeck Card Database API
  slug: ygoprodeck-card-database-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yu-gi-oh/refs/heads/main/openapi/yu-gi-oh-ygoprodeck-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "ssl.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: ygoprodeck.com
  spf: true
hosts:
- cert_expires: Sep  1 13:23:49 2026 GMT
  host: ygoprodeck.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 12 13:51:46 2026 GMT
  host: db.ygoprodeck.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Yu Gi Oh Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for YGOPRODeck, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: YGOPRODeck
provider_slug: yu-gi-oh
slug: yu-gi-oh-domain-security
source_filename: yu-gi-oh-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ygoprodeck.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  1 13:23:49 2026 GMT\n  hsts: false\n- host: db.ygoprodeck.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 12 13:51:46 2026 GMT\n  hsts: false\ndomains:\n- domain: ygoprodeck.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/yu-gi-oh/refs/heads/main/security/yu-gi-oh-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Games
- Trading Card Games
- Yu Gi Oh
- Card Database
- Open Data
- Community API
- Public APIs
---
