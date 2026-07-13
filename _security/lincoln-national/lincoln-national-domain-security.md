---
api_specs:
- filename: lincoln-national-openapi.yml
  format: yaml
  label: Lincoln Financial LincSmart Enrollment API
  slug: lincsmart-enrollment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lincoln-national/refs/heads/main/openapi/lincoln-national-openapi.yml
- filename: lincoln-national-openapi.yml
  format: yaml
  label: Lincoln Financial LincSmart EOI Solution API
  slug: lincsmart-eoi-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lincoln-national/refs/heads/main/openapi/lincoln-national-openapi.yml
- filename: lincoln-national-openapi.yml
  format: yaml
  label: Lincoln Financial LincSmart Plan Design API
  slug: lincsmart-plan-design-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lincoln-national/refs/heads/main/openapi/lincoln-national-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: lincolnfinancial.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: mylincolnportal.com
  spf: false
hosts:
- cert_expires: Oct  9 23:59:59 2026 GMT
  host: www.lincolnfinancial.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 22 23:59:59 2026 GMT
  host: www.mylincolnportal.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Lincoln National Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Lincoln National, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Lincoln National
provider_slug: lincoln-national
slug: lincoln-national-domain-security
source_filename: lincoln-national-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.lincolnfinancial.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  9 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: www.mylincolnportal.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 22 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: lincolnfinancial.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n- domain: mylincolnportal.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lincoln-national/refs/heads/main/security/lincoln-national-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Annuities
- Benefits
- Enrollment
- HR
- Insurance
- Retirement
- Fortune 500
---
