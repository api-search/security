---
api_specs:
- filename: Benefits.json
  format: json
  label: Workday Benefits API
  slug: workday-benefits-api
  spec_type: OpenAPI
  url: https://community.workday.com/sites/default/files/file-hosting/productionapi/Benefits/v40.2/Benefits.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: workday.com
  spf: true
hosts:
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
name: Workday Benefits Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Workday Benefits, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Workday Benefits
provider_slug: workday-benefits
slug: workday-benefits-domain-security
source_filename: workday-benefits-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.workday.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 23 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: wd2-impl-services1.workday.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  2 03:30:49 2026 GMT\n  hsts: null\ndomains:\n- domain: workday.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/workday-benefits/refs/heads/main/security/workday-benefits-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags: []
---
