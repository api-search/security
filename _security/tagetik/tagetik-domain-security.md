---
api_specs:
- filename: cch-tagetik-odata-openapi.yml
  format: yaml
  label: CCH Tagetik OData API
  slug: cch-tagetik-odata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tagetik/refs/heads/main/openapi/cch-tagetik-odata-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: wolterskluwer.com
  spf: true
hosts:
- cert_expires: Aug 15 14:28:43 2026 GMT
  host: www.wolterskluwer.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Tagetik Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CCH Tagetik, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: CCH Tagetik
provider_slug: tagetik
slug: tagetik-domain-security
source_filename: tagetik-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.wolterskluwer.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 15 14:28:43 2026 GMT\n  hsts: null\ndomains:\n- domain: wolterskluwer.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tagetik/refs/heads/main/security/tagetik-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Analytics
- Budgeting
- Corporate Performance Management
- ESG
- Financial Close
- Financial Consolidation
- Financial Planning
- OData
- Reporting
---
