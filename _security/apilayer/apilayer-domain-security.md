---
description: ''
domains:
- caa:
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: apilayer.com
  spf: true
hosts:
- cert_expires: Aug 12 16:33:32 2026 GMT
  host: apilayer.com
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 12 16:33:32 2026 GMT
  host: api.apilayer.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Apilayer Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for APILayer, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: APILayer
provider_slug: apilayer
slug: apilayer-domain-security
source_filename: apilayer-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: apilayer.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 12 16:33:32 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\n- host: api.apilayer.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 12 16:33:32 2026 GMT\n  hsts: null\ndomains:\n- domain: apilayer.com\n  dnssec: false\n  caa:\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/apilayer/refs/heads/main/security/apilayer-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- API Catalog
- API Discovery
- API Marketplace
- Developer Tools
- SaaS APIs
---
