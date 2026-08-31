---
api_specs:
- filename: openenvoy-job-api-openapi.yml
  format: yaml
  label: OpenEnvoy Job API
  slug: openenvoy-job-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openenvoy/refs/heads/main/openapi/openenvoy-job-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: openenvoy.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: openenvoy.io
  spf: false
hosts:
- cert_expires: Nov 20 08:21:35 2026 GMT
  host: www.openenvoy.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  8 02:36:58 2026 GMT
  host: apidocs.openenvoy.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar 11 23:59:59 2027 GMT
  host: backend.openenvoy.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Openenvoy Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for OpenEnvoy, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: OpenEnvoy
provider_slug: openenvoy
slug: openenvoy-domain-security
source_filename: openenvoy-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.openenvoy.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 20 08:21:35 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: apidocs.openenvoy.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  8 02:36:58 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: backend.openenvoy.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 11 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: openenvoy.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: openenvoy.io\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/openenvoy/refs/heads/main/security/openenvoy-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Accounts Payable
- Accounts Receivable
- Invoice Processing
- Finance Automation
- Accounting
- Procure to Pay
- Document Processing
- Artificial Intelligence
- ERP Integration
- Spend Management
---
