---
api_specs:
- filename: liquid-m-ads-api-openapi.yml
  format: yaml
  label: Liquid M Ads API
  slug: liquid-m-ads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/liquid-m/refs/heads/main/openapi/liquid-m-ads-api-openapi.yml
- filename: liquid-m-authentication-api-openapi.yml
  format: yaml
  label: Liquid M Authentication API
  slug: liquid-m-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/liquid-m/refs/heads/main/openapi/liquid-m-authentication-api-openapi.yml
- filename: liquid-m-budgets-api-openapi.yml
  format: yaml
  label: Liquid M Budgets API
  slug: liquid-m-budgets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/liquid-m/refs/heads/main/openapi/liquid-m-budgets-api-openapi.yml
- filename: liquid-m-campaigns-api-openapi.yml
  format: yaml
  label: Liquid M Campaigns API
  slug: liquid-m-campaigns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/liquid-m/refs/heads/main/openapi/liquid-m-campaigns-api-openapi.yml
- filename: liquid-m-reporting-api-openapi.yml
  format: yaml
  label: Liquid M Reporting API
  slug: liquid-m-reporting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/liquid-m/refs/heads/main/openapi/liquid-m-reporting-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: liquidm.com
  spf: true
hosts:
- host: liquidm.com
  hsts: null
  https: true
  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: certificate has expired (_ssl.c:1082)'
- cert_expires: Oct  2 08:04:11 2026 GMT
  host: platform.liquidm.com
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Liquid M Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Liquid M, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Liquid M
provider_slug: liquid-m
slug: liquid-m-domain-security
source_filename: liquid-m-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: liquidm.com\n  https: true\n  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: certificate has\n    expired (_ssl.c:1082)'\n  hsts: null\n- host: platform.liquidm.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct  2 08:04:11 2026 GMT\n  hsts: false\ndomains:\n- domain: liquidm.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/liquid-m/refs/heads/main/security/liquid-m-domain-security.yml
summary_line: TLSv1.2
tags:
- Company
- Advertising
- AdTech
- Demand-Side Platform
- Programmatic Advertising
- Mobile Advertising
- Reporting
- Analytics
- Campaign Management
- OpenRTB
---
