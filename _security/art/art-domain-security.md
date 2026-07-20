---
api_specs:
- filename: art-openapi.yml
  format: yaml
  label: Artsy Public API
  slug: artsy-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/art/refs/heads/main/openapi/art-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "sectigo.com"
  - 0 issue "ssl.com"
  - 0 issuewild "amazon.com"
  - 0 issuewild "comodoca.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: artsy.net
  spf: true
hosts:
- cert_expires: Aug 22 03:05:15 2026 GMT
  host: www.artsy.net
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 22 03:05:15 2026 GMT
  host: developers.artsy.net
  hsts: true
  hsts_max_age: 15724800
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 22 03:05:15 2026 GMT
  host: api.artsy.net
  hsts: true
  hsts_max_age: 15724800
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Art Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Artsy, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Artsy
provider_slug: art
slug: art-domain-security
source_filename: art-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.artsy.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 22 03:05:15 2026 GMT\n  hsts: null\n- host: developers.artsy.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 22 03:05:15 2026 GMT\n  hsts: true\n  hsts_max_age: 15724800\n- host: api.artsy.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 22 03:05:15 2026 GMT\n  hsts: true\n  hsts_max_age: 15724800\ndomains:\n- domain: artsy.net\n  dnssec: true\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"amazon.com\"\n  - 0 issuewild \"comodoca.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/art/refs/heads/main/security/art-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Art
- Marketplace
- Culture
- Museums
- Galleries
- Auctions
- Media
- Hypermedia
- Company
---
