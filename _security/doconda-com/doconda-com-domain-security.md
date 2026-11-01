---
api_specs:
- filename: doconda-com-dashboard-api-openapi.yml
  format: yaml
  label: doconda-com Dashboard API
  slug: doconda-com-dashboard-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/doconda-com/openapi/doconda-com-dashboard-api-openapi.yml
- filename: doconda-com-documents-api-openapi.yml
  format: yaml
  label: doconda-com Documents API
  slug: doconda-com-documents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/doconda-com/openapi/doconda-com-documents-api-openapi.yml
- filename: doconda-com-editor-api-openapi.yml
  format: yaml
  label: doconda-com Editor API
  slug: doconda-com-editor-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/doconda-com/openapi/doconda-com-editor-api-openapi.yml
- filename: doconda-com-files-api-openapi.yml
  format: yaml
  label: doconda-com Files API
  slug: doconda-com-files-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/doconda-com/openapi/doconda-com-files-api-openapi.yml
- filename: doconda-com-webhooks-api-openapi.yml
  format: yaml
  label: doconda-com Webhooks API
  slug: doconda-com-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/doconda-com/openapi/doconda-com-webhooks-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: doconda.com
  spf: true
hosts:
- cert_expires: Apr 18 23:59:59 2027 GMT
  host: doconda.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Doconda Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for doconda-com, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: doconda-com
provider_slug: doconda-com
slug: doconda-com-domain-security
source_filename: doconda-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: doconda.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Apr 18 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: doconda.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/doconda-com/security/doconda-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Document Generation
- API
- Conversion
- Automation
- AI
---
