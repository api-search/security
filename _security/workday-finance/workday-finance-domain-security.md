---
api_specs:
- filename: workday-finance-financial-management-openapi.yml
  format: yaml
  label: Workday Financial Management API
  slug: workday-financial-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday-finance/refs/heads/main/openapi/workday-finance-financial-management-openapi.yml
- filename: workday-finance-procurement-openapi.yml
  format: yaml
  label: Workday Resource Management API
  slug: workday-resource-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday-finance/refs/heads/main/openapi/workday-finance-procurement-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: workday.com
  spf: true
hosts:
- cert_expires: Sep 10 23:59:59 2026 GMT
  host: community.workday.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 23 23:59:59 2026 GMT
  host: www.workday.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  2 03:30:49 2026 GMT
  host: wd2-impl-services1.workday.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Workday Finance Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Workday Finance, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Workday Finance
provider_slug: workday-finance
slug: workday-finance-domain-security
source_filename: workday-finance-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: community.workday.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 10 23:59:59 2026 GMT\n  hsts: null\n- host: www.workday.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 23 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: wd2-impl-services1.workday.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  2 03:30:49 2026 GMT\n  hsts: null\ndomains:\n- domain: workday.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/workday-finance/refs/heads/main/security/workday-finance-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Accounting
- Cloud
- Enterprise
- ERP
- Finance
- Financial Management
---
