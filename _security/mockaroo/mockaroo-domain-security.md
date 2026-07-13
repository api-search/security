---
api_specs:
- filename: mockaroo-openapi.yml
  format: yaml
  label: Mockaroo API
  slug: mockaroo
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mockaroo/refs/heads/main/openapi/mockaroo-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: mockaroo.com
  spf: false
hosts:
- cert_expires: Sep 19 23:00:20 2026 GMT
  host: www.mockaroo.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 19 23:00:20 2026 GMT
  host: api.mockaroo.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Mockaroo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Mockaroo, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: Mockaroo
provider_slug: mockaroo
slug: mockaroo-domain-security
source_filename: mockaroo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.mockaroo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 19 23:00:20 2026 GMT\n  hsts: false\n- host: api.mockaroo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 19 23:00:20 2026 GMT\n  hsts: null\ndomains:\n- domain: mockaroo.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mockaroo/refs/heads/main/security/mockaroo-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Test Data
- Mock Data
- API Mocking
- Data Generation
- Developer Tools
- QA Testing
- Realistic Data
- Schemas
- Datasets
- Public APIs
---
