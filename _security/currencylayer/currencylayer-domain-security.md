---
api_specs:
- filename: currencylayer-openapi.yml
  format: yaml
  label: Currencylayer API
  slug: currencylayer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/currencylayer/refs/heads/main/openapi/currencylayer-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: currencylayer.com
  spf: false
- caa:
  - 0 issue "ssl.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: apilayer.com
  spf: true
hosts:
- cert_expires: Aug 15 18:54:04 2026 GMT
  host: currencylayer.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 12 16:33:32 2026 GMT
  host: api.apilayer.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 15 18:54:04 2026 GMT
  host: api.currencylayer.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Currencylayer Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Currencylayer, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: Currencylayer
provider_slug: currencylayer
slug: currencylayer-domain-security
source_filename: currencylayer-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: currencylayer.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 15 18:54:04 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.apilayer.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 12 16:33:32 2026 GMT\n  hsts: null\n- host: api.currencylayer.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 15 18:54:04 2026 GMT\n  hsts: null\ndomains:\n- domain: currencylayer.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n- domain: apilayer.com\n  dnssec: false\n  caa:\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/currencylayer/refs/heads/main/security/currencylayer-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Currency Exchange
- Foreign Exchange
- FX
- Forex
- Conversion
- Historical Rates
- Time Frame
- Change Report
- Precious Metals
- APILayer
- Public APIs
---
