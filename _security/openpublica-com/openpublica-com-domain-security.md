---
api_specs:
- filename: openpublica-com-corpus-api-openapi.yml
  format: yaml
  label: Open Publica Corpus API
  slug: openpublica-com-corpus-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/openpublica-com/openapi/openpublica-com-corpus-api-openapi.yml
- filename: openpublica-com-documents-api-openapi.yml
  format: yaml
  label: Open Publica Documents API
  slug: openpublica-com-documents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/openpublica-com/openapi/openpublica-com-documents-api-openapi.yml
- filename: openpublica-com-governments-api-openapi.yml
  format: yaml
  label: Open Publica Governments API
  slug: openpublica-com-governments-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/openpublica-com/openapi/openpublica-com-governments-api-openapi.yml
- filename: openpublica-com-meetings-api-openapi.yml
  format: yaml
  label: Open Publica Meetings API
  slug: openpublica-com-meetings-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/openpublica-com/openapi/openpublica-com-meetings-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  - 0 issue "amazon.com"
  - 0 issue "letsencrypt.org"
  dmarc: false
  dnssec: false
  domain: openpublica.com
  spf: false
hosts:
- cert_expires: Feb  8 21:55:08 2027 GMT
  host: openpublica.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Open Publica Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Open Publica, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Open Publica
provider_slug: openpublica-com
slug: openpublica-com-domain-security
source_filename: openpublica-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: openpublica.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  8 21:55:08 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: openpublica.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/openpublica-com/security/openpublica-com-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- OpenPublica
- Civic Tech
- Transparency
- Meetings
- Summary
---
