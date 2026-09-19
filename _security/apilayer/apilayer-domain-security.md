---
api_specs:
- filename: apilayer-endpoints-api-openapi.yml
  format: yaml
  label: APILayer Endpoints API
  slug: apilayer-endpoints-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apilayer/refs/heads/main/openapi/apilayer-endpoints-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 issue "amazon.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: apilayer.com
  spf: true
- caa:
  - 0 issue "ssl.com"
  - 0 issuewild "amazonaws.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: exchangerate.host
  spf: true
hosts:
- cert_expires: Dec  8 20:19:12 2026 GMT
  host: apilayer.com
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  8 20:19:12 2026 GMT
  host: api.apilayer.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 18 12:46:50 2026 GMT
  host: api.exchangerate.host
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Apilayer Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for APILayer, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: APILayer
provider_slug: apilayer
slug: apilayer-domain-security
source_filename: apilayer-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: apilayer.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  8 20:19:12 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\n- host: api.apilayer.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  8 20:19:12 2026 GMT\n  hsts: null\n- host: api.exchangerate.host\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 18 12:46:50 2026 GMT\n  hsts: null\ndomains:\n- domain: apilayer.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: exchangerate.host\n  dnssec: false\n  caa:\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"amazonaws.com\"\n  - 0 issuewild \"comodoca.com\"\
  \n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/apilayer/refs/heads/main/security/apilayer-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- API Marketplace
- API Catalog
- API Discovery
- Developer Tools
- SaaS APIs
- Geolocation
- Currency
- Data API
---
