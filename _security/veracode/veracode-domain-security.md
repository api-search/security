---
api_specs:
- filename: veracode-applications-openapi.yml
  format: yaml
  label: Veracode Applications REST API
  slug: veracode-applications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/veracode/refs/heads/main/openapi/veracode-applications-openapi.yml
- filename: veracode-findings-openapi.yml
  format: yaml
  label: Veracode Findings REST API
  slug: veracode-findings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/veracode/refs/heads/main/openapi/veracode-findings-openapi.yml
- filename: veracode-identity-openapi.yml
  format: yaml
  label: Veracode Identity REST API
  slug: veracode-identity-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/veracode/refs/heads/main/openapi/veracode-identity-openapi.yml
- filename: veracode-reporting-openapi.yml
  format: yaml
  label: Veracode Reporting REST API
  slug: veracode-reporting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/veracode/refs/heads/main/openapi/veracode-reporting-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: veracode.com
  spf: true
hosts:
- cert_expires: Aug 23 22:47:36 2026 GMT
  host: www.veracode.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 28 14:49:07 2026 GMT
  host: docs.veracode.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 28 14:49:07 2026 GMT
  host: api.veracode.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Veracode Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Veracode, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Veracode
provider_slug: veracode
slug: veracode-domain-security
source_filename: veracode-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.veracode.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 23 22:47:36 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.veracode.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 14:49:07 2026 GMT\n  hsts: false\n- host: api.veracode.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 14:49:07 2026 GMT\n  hsts: null\ndomains:\n- domain: veracode.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/veracode/refs/heads/main/security/veracode-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Application Security
- SAST
- DAST
- SCA
- Security Testing
- DevSecOps
---
