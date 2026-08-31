---
api_specs:
- filename: datavant-configuration-api-openapi.yml
  format: yaml
  label: Datavant Configuration API
  slug: datavant-configuration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/datavant/refs/heads/main/openapi/datavant-configuration-api-openapi.yml
- filename: datavant-documents-api-openapi.yml
  format: yaml
  label: Datavant Documents API
  slug: datavant-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/datavant/refs/heads/main/openapi/datavant-documents-api-openapi.yml
- filename: datavant-oauth2-api-openapi.yml
  format: yaml
  label: Datavant Oauth2 API
  slug: datavant-oauth2-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/datavant/refs/heads/main/openapi/datavant-oauth2-api-openapi.yml
- filename: datavant-order-queries-api-openapi.yml
  format: yaml
  label: Datavant Order Queries API
  slug: datavant-order-queries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/datavant/refs/heads/main/openapi/datavant-order-queries-api-openapi.yml
- filename: datavant-orders-api-openapi.yml
  format: yaml
  label: Datavant Orders API
  slug: datavant-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/datavant/refs/heads/main/openapi/datavant-orders-api-openapi.yml
- filename: datavant-prematch-api-openapi.yml
  format: yaml
  label: Datavant Prematch API
  slug: datavant-prematch-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/datavant/refs/heads/main/openapi/datavant-prematch-api-openapi.yml
- filename: datavant-projects-api-openapi.yml
  format: yaml
  label: Datavant Projects API
  slug: datavant-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/datavant/refs/heads/main/openapi/datavant-projects-api-openapi.yml
- filename: datavant-visits-api-openapi.yml
  format: yaml
  label: Datavant Visits API
  slug: datavant-visits-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/datavant/refs/heads/main/openapi/datavant-visits-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: datavant.com
  spf: true
- caa: []
  dmarc: false
  dnssec: true
  domain: datavant.io
  spf: false
hosts:
- cert_expires: Sep 16 02:30:59 2026 GMT
  host: www.datavant.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 18 23:59:59 2026 GMT
  host: api.datavant.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Datavant Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Datavant, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Datavant
provider_slug: datavant
slug: datavant-domain-security
source_filename: datavant-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-14'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.datavant.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 02:30:59 2026 GMT\n  hsts: false\n- host: api.datavant.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 18 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: datavant.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: datavant.io\n  dnssec: true\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/datavant/refs/heads/main/security/datavant-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Healthcare
- United States
- Interoperability
- Health Data
- De-Identification
- Tokenization
- Real-World Data
- Record Retrieval
- Data Connectivity
- Life Sciences
- HIPAA
- Medical Records
- Release of Information
- Privacy
- Authentication
- Health Information Exchange
---
