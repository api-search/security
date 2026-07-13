---
api_specs:
- filename: entso-e-openapi.yml
  format: yaml
  label: ENTSO-E Day-Ahead Prices API
  slug: entso-e-day-ahead-prices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/entso-e/refs/heads/main/openapi/entso-e-openapi.yml
- filename: entso-e-openapi.yml
  format: yaml
  label: ENTSO-E Load API
  slug: entso-e-load-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/entso-e/refs/heads/main/openapi/entso-e-openapi.yml
- filename: entso-e-openapi.yml
  format: yaml
  label: ENTSO-E Generation API
  slug: entso-e-generation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/entso-e/refs/heads/main/openapi/entso-e-openapi.yml
- filename: entso-e-openapi.yml
  format: yaml
  label: ENTSO-E Balancing API
  slug: entso-e-balancing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/entso-e/refs/heads/main/openapi/entso-e-openapi.yml
- filename: entso-e-openapi.yml
  format: yaml
  label: ENTSO-E Transmission API
  slug: entso-e-transmission-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/entso-e/refs/heads/main/openapi/entso-e-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: entsoe.eu
  spf: true
- caa:
  - 0 issue "amazon.com"
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "amazon.com"
  - 0 issuewild "digicert.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: getpostman.com
  spf: true
hosts:
- cert_expires: Mar 13 23:59:59 2027 GMT
  host: www.entsoe.eu
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar 13 23:59:59 2027 GMT
  host: transparency.entsoe.eu
  hsts: true
  hsts_max_age: 15724800
  https: true
  tls_version: TLSv1.2
- cert_expires: Sep 16 04:02:05 2026 GMT
  host: documenter.getpostman.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Entso E Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ENTSO-E, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: ENTSO-E
provider_slug: entso-e
slug: entso-e-domain-security
source_filename: entso-e-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.entsoe.eu\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 13 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: transparency.entsoe.eu\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Mar 13 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 15724800\n- host: documenter.getpostman.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 04:02:05 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: entsoe.eu\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: getpostman.com\n  dnssec: false\n  caa:\n  - 0 issue \"amazon.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"amazon.com\"\n  - 0 issuewild \"digicert.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/entso-e/refs/heads/main/security/entso-e-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Electricity
- Energy
- Energy Markets
- Day-Ahead Prices
- Balancing
- Transmission
- Grid Data
- Europe
---
