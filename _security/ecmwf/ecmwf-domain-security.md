---
api_specs:
- filename: ecmwf-data-stores-processing-openapi.yml
  format: yaml
  label: ECMWF Data Stores Processing API
  slug: ecmwf-data-stores-processing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ecmwf/openapi/ecmwf-data-stores-processing-openapi.yml
- filename: ecmwf-data-stores-catalogue-openapi.yml
  format: yaml
  label: ECMWF Data Stores STAC Catalogue API
  slug: ecmwf-data-stores-stac-catalogue-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ecmwf/openapi/ecmwf-data-stores-catalogue-openapi.yml
- filename: ecmwf-data-stores-profiles-openapi.yml
  format: yaml
  label: ECMWF Data Stores Profile API
  slug: ecmwf-data-stores-profile-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ecmwf/openapi/ecmwf-data-stores-profiles-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "digicert.com"
  - 0 issue "sectigo.com"
  - 0 issuewild "sectigo.com"
  - 0 issuewild "harica.gr"
  - 0 issue "harica.gr"
  - 0 issue "amazonaws.com"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: ecmwf.int
  spf: true
hosts:
- cert_expires: Nov 11 13:28:13 2026 GMT
  host: ecmwf.int
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Ecmwf Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ECMWF, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: ECMWF
provider_slug: ecmwf
slug: ecmwf-domain-security
source_filename: ecmwf-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ecmwf.int\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 11 13:28:13 2026 GMT\n  hsts: false\ndomains:\n- domain: ecmwf.int\n  dnssec: false\n  caa:\n  - 0 issuewild \"digicert.com\"\n  - 0 issue \"sectigo.com\"\n  - 0 issuewild \"sectigo.com\"\n  - 0 issuewild \"harica.gr\"\n  - 0 issue \"harica.gr\"\n  - 0 issue \"amazonaws.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/ecmwf/security/ecmwf-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Weather
- Meteorology
- Forecasting
- Climate
- Open Data
- Research
- Intergovernmental
---
