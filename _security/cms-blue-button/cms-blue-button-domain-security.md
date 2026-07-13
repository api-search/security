---
api_specs:
- filename: cms-blue-button-openapi.yml
  format: yaml
  label: CMS Blue Button 2.0 Explanation of Benefit API
  slug: cms-blue-button-explanation-of-benefit-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cms-blue-button/refs/heads/main/openapi/cms-blue-button-openapi.yml
- filename: cms-blue-button-openapi.yml
  format: yaml
  label: CMS Blue Button 2.0 Patient API
  slug: cms-blue-button-patient-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cms-blue-button/refs/heads/main/openapi/cms-blue-button-openapi.yml
- filename: cms-blue-button-openapi.yml
  format: yaml
  label: CMS Blue Button 2.0 Coverage API
  slug: cms-blue-button-coverage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cms-blue-button/refs/heads/main/openapi/cms-blue-button-openapi.yml
- filename: cms-blue-button-openapi.yml
  format: yaml
  label: CMS Blue Button 2.0 Authorization and UserInfo API
  slug: cms-blue-button-authorization-userinfo-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cms-blue-button/refs/heads/main/openapi/cms-blue-button-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: cms.gov
  spf: true
hosts:
- cert_expires: Jan 22 23:59:59 2027 GMT
  host: bluebutton.cms.gov
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 22 23:59:59 2027 GMT
  host: api.bluebutton.cms.gov
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  3 17:49:24 2026 GMT
  host: sandbox.bluebutton.cms.gov
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Cms Blue Button Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CMS Blue Button 2.0, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: CMS Blue Button 2.0
provider_slug: cms-blue-button
slug: cms-blue-button-domain-security
source_filename: cms-blue-button-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: bluebutton.cms.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 22 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.bluebutton.cms.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 22 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: sandbox.bluebutton.cms.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  3 17:49:24 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: cms.gov\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cms-blue-button/refs/heads/main/security/cms-blue-button-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Blue Button
- CARIN
- Medicare
- FHIR
- Claims Data
- Patient Access
- Healthcare
- Government
---
