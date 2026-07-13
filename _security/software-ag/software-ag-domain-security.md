---
api_specs:
- filename: webmethods-api-gateway-openapi.yml
  format: yaml
  label: webMethods API Gateway Service Management API
  slug: webmethods-api-gateway
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/software-ag/refs/heads/main/openapi/webmethods-api-gateway-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: softwareag.com
  spf: true
hosts:
- host: developer.softwareag.com
  hsts: null
  https: true
  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: unable to get local issuer certificate (_ssl.c:1082)'
- cert_expires: Aug 29 14:58:40 2026 GMT
  host: www.softwareag.com
  hsts: true
  hsts_max_age: 300
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 26 08:38:54 2026 GMT
  host: documentation.softwareag.com
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Software Ag Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Software AG, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Software AG
provider_slug: software-ag
slug: software-ag-domain-security
source_filename: software-ag-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developer.softwareag.com\n  https: true\n  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: unable to get\n    local issuer certificate (_ssl.c:1082)'\n  hsts: null\n- host: www.softwareag.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 29 14:58:40 2026 GMT\n  hsts: true\n  hsts_max_age: 300\n- host: documentation.softwareag.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec 26 08:38:54 2026 GMT\n  hsts: false\ndomains:\n- domain: softwareag.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/software-ag/refs/heads/main/security/software-ag-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- API Management
- Enterprise Integration
- iPaaS
- webMethods
- Integration Platform
- API Gateway
---
