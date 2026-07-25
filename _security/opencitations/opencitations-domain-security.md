---
api_specs:
- filename: opencitations-authors-api-openapi.yml
  format: yaml
  label: OpenCitations Authors API
  slug: opencitations-authors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opencitations/refs/heads/main/openapi/opencitations-authors-api-openapi.yml
- filename: opencitations-citations-api-openapi.yml
  format: yaml
  label: OpenCitations Citations API
  slug: opencitations-citations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opencitations/refs/heads/main/openapi/opencitations-citations-api-openapi.yml
- filename: opencitations-editors-api-openapi.yml
  format: yaml
  label: OpenCitations Editors API
  slug: opencitations-editors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opencitations/refs/heads/main/openapi/opencitations-editors-api-openapi.yml
- filename: opencitations-metadata-api-openapi.yml
  format: yaml
  label: OpenCitations Metadata API
  slug: opencitations-metadata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opencitations/refs/heads/main/openapi/opencitations-metadata-api-openapi.yml
- filename: opencitations-references-api-openapi.yml
  format: yaml
  label: OpenCitations References API
  slug: opencitations-references-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opencitations/refs/heads/main/openapi/opencitations-references-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: opencitations.net
  spf: true
hosts:
- cert_expires: Sep  8 06:53:26 2026 GMT
  host: api.opencitations.net
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 30 23:02:50 2026 GMT
  host: sparql.opencitations.net
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Opencitations Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for OpenCitations, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: OpenCitations
provider_slug: opencitations
slug: opencitations-domain-security
source_filename: opencitations-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: api.opencitations.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  8 06:53:26 2026 GMT\n  hsts: false\n- host: sparql.opencitations.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 30 23:02:50 2026 GMT\n  hsts: false\ndomains:\n- domain: opencitations.net\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/opencitations/refs/heads/main/security/opencitations-domain-security.yml
summary_line: TLSv1.3
tags:
- Citations
- Scholarly
- Research
- Open Science
- Bibliometrics
- DOI
- Academic
---
