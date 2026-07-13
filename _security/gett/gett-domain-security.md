---
api_specs:
- filename: openapi.yml
  format: yaml
  label: Gett Business API
  slug: gett-business-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gett/refs/heads/main/openapi/openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "amazonaws.com"
  - 0 issuewild "amazontrust.com"
  - 0 issuewild "awstrust.com"
  - 0 issuewild "digicert.com"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: gett.com
  spf: true
hosts:
- cert_expires: Oct  2 15:00:01 2026 GMT
  host: developer.gett.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  7 17:59:18 2026 GMT
  host: business-api.gett.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Gett Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Gett, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Gett
provider_slug: gett
slug: gett-domain-security
source_filename: gett-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developer.gett.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 15:00:01 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: business-api.gett.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  7 17:59:18 2026 GMT\n  hsts: null\ndomains:\n- domain: gett.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"amazonaws.com\"\n  - 0 issuewild \"amazontrust.com\"\n  - 0 issuewild \"awstrust.com\"\n  - 0 issuewild \"digicert.com\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gett/refs/heads/main/security/gett-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Ground Transportation
- Corporate Travel
- Ride Booking
- Business Travel
- Expense Management
---
