---
api_specs:
- filename: nedap-ons-openapi-original.json
  format: json
  label: Nedap Ons API
  slug: nedap-ons-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nedap/refs/heads/main/openapi/nedap-ons-openapi-original.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: nedap.com
  spf: true
- caa:
  - 0 issue "amazon.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: ons-api.nl
  spf: true
hosts:
- cert_expires: Nov 19 13:04:14 2026 GMT
  host: www.nedap.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb  2 23:59:59 2027 GMT
  host: ons-api.nl
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 15 23:59:59 2026 GMT
  host: api.ons.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Nedap Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Nedap, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Nedap
provider_slug: nedap
slug: nedap-domain-security
source_filename: nedap-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.nedap.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 19 13:04:14 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: ons-api.nl\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  2 23:59:59 2027 GMT\n  hsts: false\n- host: api.ons.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 15 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: nedap.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: ons-api.nl\n  dnssec: false\n  caa:\n  - 0 issue \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nedap/refs/heads/main/security/nedap-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Healthcare
- Electronic Health Records
- Interoperability
- FHIR
- openEHR
- RFID
- Retail
- Physical Security
- Livestock
- Netherlands
- Webhooks
---
