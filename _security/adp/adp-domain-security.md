---
api_specs:
- filename: adp-workers-openapi.yml
  format: yaml
  label: ADP Workers API
  slug: adp-workers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adp/refs/heads/main/openapi/adp-workers-openapi.yml
- filename: adp-payroll-openapi.yml
  format: yaml
  label: ADP Payroll API
  slug: adp-payroll-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adp/refs/heads/main/openapi/adp-payroll-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: adp.com
  spf: true
hosts:
- cert_expires: Dec 23 23:59:59 2026 GMT
  host: developers.adp.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 27 23:59:59 2026 GMT
  host: api.adp.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Adp Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ADP, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: ADP
provider_slug: adp
slug: adp-domain-security
source_filename: adp-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developers.adp.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 23 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.adp.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 27 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: adp.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/adp/refs/heads/main/security/adp-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Benefits
- HCM
- HR
- Payroll
- Workforce
---
