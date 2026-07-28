---
api_specs:
- filename: northern-powergrid-open-data-explore-api-v2-1-openapi.json
  format: json
  label: Northern Powergrid Open Data Explore API
  slug: northern-powergrid-open-data-explore-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/northern-powergrid/refs/heads/main/openapi/northern-powergrid-open-data-explore-api-v2-1-openapi.json
- filename: northern-powergrid-open-data-explore-api-v2-0-openapi.json
  format: json
  label: Northern Powergrid Open Data Explore API v2.0
  slug: northern-powergrid-open-data-explore-api-v2-0
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/northern-powergrid/refs/heads/main/openapi/northern-powergrid-open-data-explore-api-v2-0-openapi.json
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
  dmarc_policy: reject
  dnssec: true
  domain: northernpowergrid.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: opendatasoft.com
  spf: true
hosts:
- cert_expires: Nov 22 23:59:59 2026 GMT
  host: www.northernpowergrid.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 17 21:02:03 2026 GMT
  host: northernpowergrid.opendatasoft.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Northern Powergrid Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Northern Powergrid, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Northern Powergrid
provider_slug: northern-powergrid
slug: northern-powergrid-domain-security
source_filename: northern-powergrid-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.northernpowergrid.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 22 23:59:59 2026 GMT\n  hsts: null\n- host: northernpowergrid.opendatasoft.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 17 21:02:03 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: northernpowergrid.com\n  dnssec: true\n  caa:\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: opendatasoft.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/northern-powergrid/refs/heads/main/security/northern-powergrid-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Energy
- United Kingdom
- Utilities
- Electricity
- Grid
- Open Data
- Distribution Network Operator
- Smart Metering
- Network Capacity
- Flexibility
- DER
- Renewables
---
