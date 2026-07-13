---
api_specs:
- filename: teco-energy-outage-openapi.yml
  format: yaml
  label: Tampa Electric Outage API
  slug: outage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/teco-energy/refs/heads/main/openapi/teco-energy-outage-openapi.yml
- filename: teco-energy-account-openapi.yml
  format: yaml
  label: Tampa Electric Account API
  slug: account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/teco-energy/refs/heads/main/openapi/teco-energy-account-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "geotrust.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "sectigo.com"
  - 0 issue " pki.goog; cansignhttpexchanges=yes"
  - 0 issue "amazonaws.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: tecoenergy.com
  spf: true
- caa:
  - 0 issue "geotrust.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: tampaelectric.com
  spf: true
hosts:
- cert_expires: Feb 23 23:59:59 2027 GMT
  host: www.tecoenergy.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 24 23:59:59 2027 GMT
  host: www.tampaelectric.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 17 23:59:59 2026 GMT
  host: account.tecoenergy.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Teco Energy Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for TECO Energy, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: TECO Energy
provider_slug: teco-energy
slug: teco-energy-domain-security
source_filename: teco-energy-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.tecoenergy.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 23 23:59:59 2027 GMT\n  hsts: false\n- host: www.tampaelectric.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 24 23:59:59 2027 GMT\n  hsts: false\n- host: account.tecoenergy.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec 17 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: tecoenergy.com\n  dnssec: false\n  caa:\n  - 0 issue \"geotrust.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \" pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: tampaelectric.com\n  dnssec: false\n  caa:\n  - 0 issue \"geotrust.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy:\
  \ reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/teco-energy/refs/heads/main/security/teco-energy-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Energy
- Utilities
- Electric
- Natural Gas
- Smart Grid
- Tampa Bay
- Fortune 1000
---
