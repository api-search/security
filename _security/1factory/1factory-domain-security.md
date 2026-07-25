---
api_specs:
- filename: 1factory-customers-api-openapi.yml
  format: yaml
  label: 1Factory Customers API
  slug: 1factory-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/1factory/refs/heads/main/openapi/1factory-customers-api-openapi.yml
- filename: 1factory-manufacturing-api-openapi.yml
  format: yaml
  label: 1Factory Manufacturing API
  slug: 1factory-manufacturing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/1factory/refs/heads/main/openapi/1factory-manufacturing-api-openapi.yml
- filename: 1factory-part-master-api-openapi.yml
  format: yaml
  label: 1Factory Part Master API
  slug: 1factory-part-master-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/1factory/refs/heads/main/openapi/1factory-part-master-api-openapi.yml
- filename: 1factory-qms-api-openapi.yml
  format: yaml
  label: 1Factory QMS API
  slug: 1factory-qms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/1factory/refs/heads/main/openapi/1factory-qms-api-openapi.yml
- filename: 1factory-receiving-api-openapi.yml
  format: yaml
  label: 1Factory Receiving API
  slug: 1factory-receiving-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/1factory/refs/heads/main/openapi/1factory-receiving-api-openapi.yml
- filename: 1factory-suppliers-api-openapi.yml
  format: yaml
  label: 1Factory Suppliers API
  slug: 1factory-suppliers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/1factory/refs/heads/main/openapi/1factory-suppliers-api-openapi.yml
- filename: 1factory-work-orders-api-openapi.yml
  format: yaml
  label: 1Factory Work Orders API
  slug: 1factory-work-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/1factory/refs/heads/main/openapi/1factory-work-orders-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: 1factory.com
  spf: true
- caa: []
  dmarc: false
  dnssec: true
  domain: 1factory.co
  spf: false
hosts:
- cert_expires: Jan 13 23:59:59 2027 GMT
  host: www.1factory.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 13 23:59:59 2027 GMT
  host: www.1factory.co
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 14 11:39:46 2026 GMT
  host: val.1factory.co
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: 1Factory Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for 1Factory, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: 1Factory
provider_slug: 1factory
slug: 1factory-domain-security
source_filename: 1factory-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.1factory.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 13 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: www.1factory.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 13 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: val.1factory.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 14 11:39:46 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: 1factory.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: 1factory.co\n  dnssec: true\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/1factory/refs/heads/main/security/1factory-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Analytics
- Data Collection
- Manufacturing
- Monitoring
- Quality
---
