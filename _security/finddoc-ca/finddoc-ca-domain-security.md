---
api_specs:
- filename: finddoc-ca-clinics-api-openapi.yml
  format: yaml
  label: FindDoc Clinics API
  slug: finddoc-ca-clinics-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/finddoc-ca/openapi/finddoc-ca-clinics-api-openapi.yml
- filename: finddoc-ca-doctors-api-openapi.yml
  format: yaml
  label: FindDoc Doctors API
  slug: finddoc-ca-doctors-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/finddoc-ca/openapi/finddoc-ca-doctors-api-openapi.yml
- filename: finddoc-ca-health-api-openapi.yml
  format: yaml
  label: FindDoc Health API
  slug: finddoc-ca-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/finddoc-ca/openapi/finddoc-ca-health-api-openapi.yml
- filename: finddoc-ca-metadata-api-openapi.yml
  format: yaml
  label: FindDoc Metadata API
  slug: finddoc-ca-metadata-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/finddoc-ca/openapi/finddoc-ca-metadata-api-openapi.yml
- filename: finddoc-ca-specialists-api-openapi.yml
  format: yaml
  label: FindDoc Specialists API
  slug: finddoc-ca-specialists-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/finddoc-ca/openapi/finddoc-ca-specialists-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "sectigo.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  dmarc: false
  dnssec: false
  domain: finddoc.ca
  spf: false
hosts:
- cert_expires: Jan  5 04:35:14 2027 GMT
  host: finddoc.ca
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: FindDoc Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for FindDoc, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: FindDoc
provider_slug: finddoc-ca
slug: finddoc-ca-domain-security
source_filename: finddoc-ca-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-08'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: finddoc.ca\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  5 04:35:14 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: finddoc.ca\n  dnssec: false\n  caa:\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/finddoc-ca/security/finddoc-ca-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Healthcare
- Doctors
- Clinics
- Canada
---
