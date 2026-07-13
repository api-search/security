---
api_specs:
- filename: openclinica-openapi.yml
  format: yaml
  label: OpenClinica Authentication API
  slug: openclinica-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openclinica/refs/heads/main/openapi/openclinica-openapi.yml
- filename: openclinica-openapi.yml
  format: yaml
  label: OpenClinica Participants API
  slug: openclinica-participants-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openclinica/refs/heads/main/openapi/openclinica-openapi.yml
- filename: openclinica-openapi.yml
  format: yaml
  label: OpenClinica Study Events API
  slug: openclinica-study-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openclinica/refs/heads/main/openapi/openclinica-openapi.yml
- filename: openclinica-openapi.yml
  format: yaml
  label: OpenClinica Clinical Data API
  slug: openclinica-clinical-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openclinica/refs/heads/main/openapi/openclinica-openapi.yml
- filename: openclinica-openapi.yml
  format: yaml
  label: OpenClinica ODM Metadata API
  slug: openclinica-odm-metadata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openclinica/refs/heads/main/openapi/openclinica-openapi.yml
- filename: openclinica-openapi.yml
  format: yaml
  label: OpenClinica Bulk Operations API
  slug: openclinica-bulk-operations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openclinica/refs/heads/main/openapi/openclinica-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: openclinica.com
  spf: true
hosts:
- cert_expires: Sep 29 21:31:15 2026 GMT
  host: www.openclinica.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 20 22:35:02 2026 GMT
  host: docs.openclinica.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Openclinica Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for OpenClinica, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: OpenClinica
provider_slug: openclinica
slug: openclinica-domain-security
source_filename: openclinica-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.openclinica.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 21:31:15 2026 GMT\n  hsts: false\n- host: docs.openclinica.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 22:35:02 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: openclinica.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/openclinica/refs/heads/main/security/openclinica-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Clinical Trials
- Electronic Data Capture
- EDC
- Clinical Data Management
- CDISC ODM
- Healthcare
- Open Source
---
