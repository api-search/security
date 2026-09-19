---
api_specs:
- filename: fda-regulations-fda-data-dashboard-api-api-openapi.yml
  format: yaml
  label: FDA Regulations FDA Data Dashboard API
  slug: fda-regulations-fda-data-dashboard-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fda-regulations/refs/heads/main/openapi/fda-regulations-fda-data-dashboard-api-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: fda.gov
  spf: true
hosts:
- cert_expires: Mar 13 16:54:46 2027 GMT
  host: www.fda.gov
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 12 16:12:35 2026 GMT
  host: api-datadashboard.fda.gov
  hsts: null
  https: true
  tls_version: TLSv1.2
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: Fda Regulations Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for FDA Regulations, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: FDA Regulations
provider_slug: fda-regulations
slug: fda-regulations-domain-security
source_filename: fda-regulations-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.fda.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 13 16:54:46 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api-datadashboard.fda.gov\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov 12 16:12:35 2026 GMT\n  hsts: null\ndomains:\n- domain: fda.gov\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fda-regulations/refs/heads/main/security/fda-regulations-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Regulatory Compliance
- Healthcare
- Medical Devices
- Pharmaceuticals
- Food Safety
- Inspection
- Enforcement
- Federal-Government
- Public Data
- Import
---
