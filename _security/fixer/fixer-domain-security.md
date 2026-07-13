---
api_specs:
- filename: fixer-openapi.yml
  format: yaml
  label: Fixer API
  slug: fixer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fixer/refs/heads/main/openapi/fixer-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: fixer.io
  spf: true
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
- cert_expires: Sep  4 02:46:34 2026 GMT
  host: fixer.io
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 12 16:33:32 2026 GMT
  host: api.apilayer.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 17 23:59:59 2026 GMT
  host: data.fixer.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Fixer Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Fixer, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Fixer
provider_slug: fixer
slug: fixer-domain-security
source_filename: fixer-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: fixer.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  4 02:46:34 2026 GMT\n  hsts: false\n- host: api.apilayer.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 12 16:33:32 2026 GMT\n  hsts: null\n- host: data.fixer.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 17 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: fixer.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: apilayer.com\n  dnssec: false\n  caa:\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fixer/refs/heads/main/security/fixer-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Currency Exchange
- Foreign Exchange
- FX
- Forex
- ECB
- Conversion
- Historical Rates
- Time Series
- Fluctuation
- APILayer
- Public APIs
---
