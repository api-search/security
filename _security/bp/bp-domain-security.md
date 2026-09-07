---
api_specs:
- filename: bp-fleet-authentication-openapi.json
  format: json
  label: bp Open Fleet Authentication API
  slug: bp-fleet-authentication
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bp/refs/heads/main/openapi/bp-fleet-authentication-openapi.json
- filename: bp-fleet-card-management-openapi.json
  format: json
  label: bp Open Fleet Card Management API
  slug: bp-fleet-card-management
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bp/refs/heads/main/openapi/bp-fleet-card-management-openapi.json
- filename: bp-fleet-invoice-management-openapi.json
  format: json
  label: bp Open Fleet Invoice Management API
  slug: bp-fleet-invoice-management
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bp/refs/heads/main/openapi/bp-fleet-invoice-management-openapi.json
- filename: bp-fleet-transaction-management-openapi.json
  format: json
  label: bp Open Fleet Transaction Management API
  slug: bp-fleet-transaction-management
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bp/refs/heads/main/openapi/bp-fleet-transaction-management-openapi.json
- filename: bp-fleet-retail-site-information-openapi.json
  format: json
  label: bp Open Fleet Retail Site Information API
  slug: bp-fleet-retail-site-information
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bp/refs/heads/main/openapi/bp-fleet-retail-site-information-openapi.json
- filename: bp-fleet-aral-appconnect-openapi.json
  format: json
  label: bp Open Fleet Aral AppConnect (Pay@Pump) API
  slug: bp-fleet-aral-appconnect
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bp/refs/heads/main/openapi/bp-fleet-aral-appconnect-openapi.json
description: ''
domains:
- caa:
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  - 0 issue "www.digicert.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: bp.com
  spf: true
hosts:
- cert_expires: Mar 19 23:59:59 2027 GMT
  host: www.bp.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 27 23:59:59 2026 GMT
  host: developer.bp.com
  hsts: true
  hsts_max_age: 10886400
  https: true
  tls_version: TLSv1.3
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: Bp Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for BP, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: BP
provider_slug: bp
slug: bp-domain-security
source_filename: bp-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.bp.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 19 23:59:59 2027 GMT\n  hsts: null\n- host: developer.bp.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 27 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 10886400\ndomains:\n- domain: bp.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  - 0 issue \"www.digicert.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bp/refs/heads/main/security/bp-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Energy
- Oil
- Gas
- Renewables
- Developer Platform
- Fleet
- Fuel Cards
- Mobility
- Retail Fuel
- EV Charging
---
