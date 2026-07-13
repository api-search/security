---
api_specs:
- filename: openapi.json
  format: json
  label: Parseflow API
  slug: parseflow-api
  spec_type: OpenAPI
  url: https://parseflow-api.thankfulisland-fec0f8f2.westus2.azurecontainerapps.io/openapi.json
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: parseflow.tech
  spf: true
- caa:
  - 0 contactemail "caarecordaware@microsoft.com"
  dmarc: false
  dnssec: false
  domain: azurecontainerapps.io
  spf: false
hosts:
- cert_expires: Oct  2 03:54:26 2026 GMT
  host: docs.parseflow.tech
  hsts: false
  https: true
  tls_version: TLSv1.3
- host: parseflow-api.thankfulisland-fec0f8f2.westus2.azurecontainerapps.io
  https: false
kind: domain-security
layout: security
method: probed
name: Parseflow Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Parseflow, probed live across 2 host(s) and 2 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Parseflow
provider_slug: parseflow
slug: parseflow-domain-security
source_filename: parseflow-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: docs.parseflow.tech\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 03:54:26 2026 GMT\n  hsts: false\n- host: parseflow-api.thankfulisland-fec0f8f2.westus2.azurecontainerapps.io\n  https: false\ndomains:\n- domain: parseflow.tech\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n- domain: azurecontainerapps.io\n  dnssec: false\n  caa:\n  - 0 contactemail \"caarecordaware@microsoft.com\"\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/parseflow/refs/heads/main/security/parseflow-domain-security.yml
summary_line: TLSv1.3
tags:
- Document Parsing
- PDF
- OCR
- Text Extraction
- Document AI
- Search
- BYOK
- Async Jobs
- Webhooks
- REST
---
