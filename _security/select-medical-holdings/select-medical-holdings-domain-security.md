---
api_specs:
- filename: select-medical-holdings-fhir-r4-openapi.yml
  format: yaml
  label: Select Medical FHIR R4 API
  slug: select-medical-holdings-fhir-r4
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/select-medical-holdings/refs/heads/main/openapi/select-medical-holdings-fhir-r4-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "sectigo.com"
  - 0 issuewild "ssl.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: selectmedical.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: epichosted.com
  spf: true
hosts:
- cert_expires: Nov 19 08:41:42 2026 GMT
  host: www.selectmedical.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 29 23:59:59 2027 GMT
  host: mychart.selectmedical.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 27 23:59:59 2026 GMT
  host: epicproxy.et0948.epichosted.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Select Medical Holdings Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Select Medical Holdings, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Select Medical Holdings
provider_slug: select-medical-holdings
slug: select-medical-holdings-domain-security
source_filename: select-medical-holdings-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.selectmedical.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 19 08:41:42 2026 GMT\n  hsts: null\n- host: mychart.selectmedical.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 29 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: epicproxy.et0948.epichosted.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov 27 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: selectmedical.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"sectigo.com\"\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: epichosted.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/select-medical-holdings/refs/heads/main/security/select-medical-holdings-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Healthcare
- Hospitals
- Rehabilitation
- Patient Access
- FHIR
- Interoperability
- Electronic Health Records
- Fortune 1000
---
