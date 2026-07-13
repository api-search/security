---
api_specs:
- filename: waste-management-customer-api-openapi.yml
  format: yaml
  label: Waste Management Customer API
  slug: waste-management-customer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/waste-management/refs/heads/main/openapi/waste-management-customer-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: wm.com
  spf: true
hosts:
- cert_expires: Aug 24 19:42:41 2026 GMT
  host: www.wm.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 20 23:59:59 2027 GMT
  host: api.wm.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 20 23:59:59 2027 GMT
  host: apitest.wm.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Waste Management Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Waste Management, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Waste Management
provider_slug: waste-management
slug: waste-management-domain-security
source_filename: waste-management-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.wm.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 24 19:42:41 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.wm.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 20 23:59:59 2027 GMT\n  hsts: false\n- host: apitest.wm.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 20 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: wm.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/waste-management/refs/heads/main/security/waste-management-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Environmental Services
- Fortune 500
- Recycling
- Solid Waste
- Sustainability
- Waste Management
---
