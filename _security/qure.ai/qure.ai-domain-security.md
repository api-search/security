---
api_specs:
- filename: qure.ai-platform-api-xray-v2-er-openapi.yml
  format: yaml
  label: Qure.ai Platform API
  slug: platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qure.ai/refs/heads/main/openapi/qure.ai-platform-api-xray-v2-er-openapi.yml
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
