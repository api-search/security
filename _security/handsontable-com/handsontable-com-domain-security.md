---
api_specs:
- filename: handsontable-com-openapi-generated.yml
  format: yaml
  label: Handsontable API
  slug: handsontable-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/handsontable-com/openapi/_ae-authored/handsontable-com-openapi-generated.yml
description: ''
domains:
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
  domain: handsontable.com
  spf: true
hosts:
- cert_expires: Feb  2 10:10:19 2027 GMT
  host: handsontable.com
  hsts: true
  hsts_max_age: 15768000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Handsontable Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Handsontable, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Handsontable
provider_slug: handsontable-com
slug: handsontable-com-domain-security
source_filename: handsontable-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-10'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: handsontable.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  2 10:10:19 2027 GMT\n  hsts: true\n  hsts_max_age: 15768000\ndomains:\n- domain: handsontable.com\n  dnssec: false\n  caa:\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/handsontable-com/security/handsontable-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- JavaScript data grid
- Spreadsheet component
- HyperFormula
- Developers
- Finance
- Design Systems
- Salesforce
---
