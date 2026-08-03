---
api_specs:
- filename: clear-street-trading-api-openapi.yml
  format: yaml
  label: Clear Street Trading API
  slug: trading-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clear-street/refs/heads/main/openapi/clear-street-trading-api-openapi.yml
- filename: clear-street-studio-openapi.yml
  format: yaml
  label: Clear Street Studio API
  slug: studio-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clear-street/refs/heads/main/openapi/clear-street-studio-openapi.yml
- filename: clear-street-legacy-api-swagger.yml
  format: yaml
  label: Clear Street API (Trades and Uploads)
  slug: legacy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clear-street/refs/heads/main/openapi/clear-street-legacy-api-swagger.yml
description: ''
domains:
- caa:
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  - 0 issuewild "amazon.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "godaddy.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: clearstreet.io
  spf: true
- caa:
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  - 0 issuewild "amazon.com"
  - 0 issuewild "comodoca.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: clearstreet.com
  spf: true
hosts:
- cert_expires: Sep 25 15:10:23 2026 GMT
  host: www.clearstreet.io
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 28 23:59:59 2026 GMT
  host: docs.clearstreet.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  2 20:03:30 2026 GMT
  host: api.clearstreet.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Clear Street Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Clear Street, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Clear Street
provider_slug: clear-street
slug: clear-street-domain-security
source_filename: clear-street-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.clearstreet.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 15:10:23 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: docs.clearstreet.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 28 23:59:59 2026 GMT\n  hsts: false\n- host: api.clearstreet.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  2 20:03:30 2026 GMT\n  hsts: null\ndomains:\n- domain: clearstreet.io\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"amazon.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"godaddy.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: clearstreet.com\n  dnssec: false\n  caa:\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\
  \n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"amazon.com\"\n  - 0 issuewild \"comodoca.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/clear-street/refs/heads/main/security/clear-street-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Financial Services
- Capital Markets
- Prime Brokerage
- Trading
- Brokerage
- Clearing
- Market Data
- Fintech
- Investing
---
