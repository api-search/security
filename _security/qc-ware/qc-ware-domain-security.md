---
api_specs:
- filename: qc-ware-files-api-openapi.yml
  format: yaml
  label: QC Ware Files API
  slug: qc-ware-files-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qc-ware/refs/heads/main/openapi/qc-ware-files-api-openapi.yml
- filename: qc-ware-workflows-api-openapi.yml
  format: yaml
  label: QC Ware Workflows API
  slug: qc-ware-workflows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qc-ware/refs/heads/main/openapi/qc-ware-workflows-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: qcware.com
  spf: true
hosts:
- cert_expires: Nov  9 04:49:54 2026 GMT
  host: www.qcware.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb  6 23:59:59 2027 GMT
  host: app.promethium.qcware.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb  6 23:59:59 2027 GMT
  host: api.promethium.qcware.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Qc Ware Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for QC Ware, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: QC Ware
provider_slug: qc-ware
slug: qc-ware-domain-security
source_filename: qc-ware-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.qcware.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  9 04:49:54 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: app.promethium.qcware.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  6 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.promethium.qcware.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  6 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: qcware.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/qc-ware/refs/heads/main/security/qc-ware-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Quantum Computing
- Computational Chemistry
- Quantum Chemistry
- Drug Discovery
- Materials Science
- Scientific Computing
- GPU Computing
- Life Sciences
- Simulation
---
