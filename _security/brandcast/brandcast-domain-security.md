---
api_specs:
- filename: brandcast-account-api-openapi.yml
  format: yaml
  label: Brandcast Account API
  slug: brandcast-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brandcast/refs/heads/main/openapi/brandcast-account-api-openapi.yml
- filename: brandcast-salesforce-api-openapi.yml
  format: yaml
  label: Brandcast Salesforce API
  slug: brandcast-salesforce-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brandcast/refs/heads/main/openapi/brandcast-salesforce-api-openapi.yml
- filename: brandcast-templates-api-openapi.yml
  format: yaml
  label: Brandcast Templates API
  slug: brandcast-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brandcast/refs/heads/main/openapi/brandcast-templates-api-openapi.yml
- filename: brandcast-websites-api-openapi.yml
  format: yaml
  label: Brandcast Websites API
  slug: brandcast-websites-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brandcast/refs/heads/main/openapi/brandcast-websites-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: brandcast.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: brandcast.io
  spf: false
hosts:
- cert_expires: Dec 31 23:59:59 2026 GMT
  host: www.brandcast.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 18 23:59:59 2026 GMT
  host: developer.brandcast.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 12 23:59:59 2026 GMT
  host: api.brandcast-prod.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Brandcast Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Brandcast, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Brandcast
provider_slug: brandcast
slug: brandcast-domain-security
source_filename: brandcast-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.brandcast.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 31 23:59:59 2026 GMT\n  hsts: null\n- host: developer.brandcast.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 18 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.brandcast-prod.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 12 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: brandcast.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: brandcast.io\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/brandcast/refs/heads/main/security/brandcast-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Enterprise Software
- No-Code
- Website Builder
- Content Management
- Digital Experience
- Web Design
- Brand Management
---
