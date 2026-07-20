---
api_specs:
- filename: andel-data-exchange-openapi.yaml
  format: yaml
  label: Data Exchange API
  slug: data-exchange-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/andel/refs/heads/main/openapi/andel-data-exchange-openapi.yaml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: andel.org
  spf: true
- caa:
  - 0 issuewild "amazon.com"
  - 0 issuewild "digicert.com"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog"
  - 0 iodef "mailto:security@postman.com"
  - 0 issue "amazon.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: pstmn.io
  spf: true
hosts:
- cert_expires: Sep 11 04:25:02 2026 GMT
  host: andel.org
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- host: api.andel.org
  https: false
- cert_expires: Oct 11 07:08:52 2026 GMT
  host: 7403d846-765d-4d63-9e5c-b7f0ab21a354.mock.pstmn.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Andel Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Andel, probed live across 3 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Andel
provider_slug: andel
slug: andel-domain-security
source_filename: andel-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: andel.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 11 04:25:02 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.andel.org\n  https: false\n- host: 7403d846-765d-4d63-9e5c-b7f0ab21a354.mock.pstmn.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 11 07:08:52 2026 GMT\n  hsts: null\ndomains:\n- domain: andel.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: pstmn.io\n  dnssec: false\n  caa:\n  - 0 issuewild \"amazon.com\"\n  - 0 issuewild \"digicert.com\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog\"\n  - 0 iodef \"mailto:security@postman.com\"\n  - 0 issue \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/andel/refs/heads/main/security/andel-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Healthcare
- Pharmacy
- Pharmacy Benefits
- Drug Pricing
- Specialty Medications
- Data Exchange
- Webhooks
---
