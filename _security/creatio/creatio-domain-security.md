---
api_specs:
- filename: creatio-odata-api-openapi.yml
  format: yaml
  label: Creatio OData API
  slug: creatio-odata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/creatio/refs/heads/main/openapi/creatio-odata-api-openapi.yml
- filename: creatio-clear-bundles-api-openapi.yml
  format: yaml
  label: Creatio Clear Bundles API
  slug: creatio-clear-bundles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/creatio/refs/heads/main/openapi/creatio-clear-bundles-api-openapi.yml
- filename: creatio-minify-content-api-openapi.yml
  format: yaml
  label: Creatio Minify Content API
  slug: creatio-minify-content-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/creatio/refs/heads/main/openapi/creatio-minify-content-api-openapi.yml
- filename: creatio-odata-api-openapi.yml
  format: yaml
  label: Creatio Odata API
  slug: creatio-odata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/creatio/refs/heads/main/openapi/creatio-odata-api-openapi.yml
- filename: creatio-process-content-api-openapi.yml
  format: yaml
  label: Creatio Process Content API
  slug: creatio-process-content-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/creatio/refs/heads/main/openapi/creatio-process-content-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: creatio.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: mycreatio.com
  spf: true
hosts:
- cert_expires: Dec  8 20:49:08 2026 GMT
  host: www.creatio.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Apr  4 23:59:59 2027 GMT
  host: academy.creatio.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- host: mycreatio.com
  hsts: null
  https: true
  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch, certificate is not valid for ''mycreatio.c'
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Creatio Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Creatio, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Creatio
provider_slug: creatio
slug: creatio-domain-security
source_filename: creatio-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.creatio.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  8 20:49:08 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: academy.creatio.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Apr  4 23:59:59 2027 GMT\n  hsts: false\n- host: mycreatio.com\n  https: true\n  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch,\n    certificate is not valid for ''mycreatio.c'\n  hsts: null\ndomains:\n- domain: creatio.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: mycreatio.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/creatio/refs/heads/main/security/creatio-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Software-as-a-Service
- CRM
- No-Code
- Low-Code
- Business Process Management
- Workflow Automation
- Sales
- Marketing
- Customer Service
- OData
- AI Agents
---
