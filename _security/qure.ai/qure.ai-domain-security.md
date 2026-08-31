---
api_specs:
- filename: qure.ai-fetch-results-api-openapi.yml
  format: yaml
  label: Qure.ai Fetch Results API
  slug: qure.ai-fetch-results-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qure.ai/refs/heads/main/openapi/qure.ai-fetch-results-api-openapi.yml
- filename: qure.ai-initiate-computation-api-openapi.yml
  format: yaml
  label: Qure.ai Initiate Computation API
  slug: qure.ai-initiate-computation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qure.ai/refs/heads/main/openapi/qure.ai-initiate-computation-api-openapi.yml
- filename: qure.ai-upload-dicoms-api-openapi.yml
  format: yaml
  label: Qure.ai Upload DICOMs API
  slug: qure.ai-upload-dicoms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qure.ai/refs/heads/main/openapi/qure.ai-upload-dicoms-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: qure.ai
  spf: true
hosts:
- cert_expires: Oct 12 15:37:00 2026 GMT
  host: www.qure.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Qure.Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Qure.ai, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Qure.ai
provider_slug: qure.ai
slug: qure.ai-domain-security
source_filename: qure.ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.qure.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 12 15:37:00 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: qure.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/qure.ai/refs/heads/main/security/qure.ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Artificial Intelligence
- Healthcare
- Medical Imaging
- Radiology
- Machine Learning
- DICOM
- Diagnostics
- Clinical Decision Support
- Health Technology
- Company
---
