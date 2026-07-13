---
api_specs:
- filename: sybase-ase-rest-api-openapi.yml
  format: yaml
  label: Sybase ASE REST API
  slug: sybase-ase-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sybase/refs/heads/main/openapi/sybase-ase-rest-api-openapi.yml
- filename: openapi.json
  format: json
  label: Sybase IQ REST API
  slug: sybase-iq-rest-api
  spec_type: OpenAPI
  url: https://api.sybase.example.com/iq/v1/openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: sap.com
  spf: true
hosts:
- cert_expires: Jan 13 23:59:59 2027 GMT
  host: support.sap.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 13 23:59:59 2027 GMT
  host: www.sap.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 25 23:59:59 2026 GMT
  host: help.sap.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Sybase Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Sybase, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Sybase
provider_slug: sybase
slug: sybase-domain-security
source_filename: sybase-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: support.sap.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 13 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: www.sap.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 13 23:59:59 2027 GMT\n  hsts: null\n- host: help.sap.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 25 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: sap.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sybase/refs/heads/main/security/sybase-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Database
- Enterprise
- SAP
- SQL
---
