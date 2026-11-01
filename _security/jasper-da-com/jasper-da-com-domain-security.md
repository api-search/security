---
api_specs:
- filename: jasper-da-com-attachments-api-openapi.yml
  format: yaml
  label: Jasper Attachments API
  slug: jasper-da-com-attachments-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/jasper-da-com/openapi/jasper-da-com-attachments-api-openapi.yml
- filename: jasper-da-com-audiences-api-openapi.yml
  format: yaml
  label: Jasper Audiences API
  slug: jasper-da-com-audiences-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/jasper-da-com/openapi/jasper-da-com-audiences-api-openapi.yml
- filename: jasper-da-com-command-api-openapi.yml
  format: yaml
  label: Jasper Command API
  slug: jasper-da-com-command-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/jasper-da-com/openapi/jasper-da-com-command-api-openapi.yml
- filename: jasper-da-com-context-sources-api-openapi.yml
  format: yaml
  label: Jasper Context Sources API
  slug: jasper-da-com-context-sources-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/jasper-da-com/openapi/jasper-da-com-context-sources-api-openapi.yml
- filename: jasper-da-com-documents-api-openapi.yml
  format: yaml
  label: Jasper Documents API
  slug: jasper-da-com-documents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/jasper-da-com/openapi/jasper-da-com-documents-api-openapi.yml
- filename: jasper-da-com-geo-api-openapi.yml
  format: yaml
  label: Jasper GEO API
  slug: jasper-da-com-geo-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/jasper-da-com/openapi/jasper-da-com-geo-api-openapi.yml
- filename: jasper-da-com-image-templates-api-openapi.yml
  format: yaml
  label: Jasper Image Templates API
  slug: jasper-da-com-image-templates-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/jasper-da-com/openapi/jasper-da-com-image-templates-api-openapi.yml
- filename: jasper-da-com-images-api-openapi.yml
  format: yaml
  label: Jasper Images API
  slug: jasper-da-com-images-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/jasper-da-com/openapi/jasper-da-com-images-api-openapi.yml
- filename: jasper-da-com-knowledge-api-openapi.yml
  format: yaml
  label: Jasper Knowledge API
  slug: jasper-da-com-knowledge-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/jasper-da-com/openapi/jasper-da-com-knowledge-api-openapi.yml
- filename: jasper-da-com-products-api-openapi.yml
  format: yaml
  label: Jasper Products API
  slug: jasper-da-com-products-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/jasper-da-com/openapi/jasper-da-com-products-api-openapi.yml
- filename: jasper-da-com-projects-api-openapi.yml
  format: yaml
  label: Jasper Projects API
  slug: jasper-da-com-projects-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/jasper-da-com/openapi/jasper-da-com-projects-api-openapi.yml
- filename: jasper-da-com-styles-api-openapi.yml
  format: yaml
  label: Jasper Styles API
  slug: jasper-da-com-styles-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/jasper-da-com/openapi/jasper-da-com-styles-api-openapi.yml
- filename: jasper-da-com-tasks-api-openapi.yml
  format: yaml
  label: Jasper Tasks API
  slug: jasper-da-com-tasks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/jasper-da-com/openapi/jasper-da-com-tasks-api-openapi.yml
- filename: jasper-da-com-templates-api-openapi.yml
  format: yaml
  label: Jasper Templates API
  slug: jasper-da-com-templates-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/jasper-da-com/openapi/jasper-da-com-templates-api-openapi.yml
- filename: jasper-da-com-usage-api-openapi.yml
  format: yaml
  label: Jasper Usage API
  slug: jasper-da-com-usage-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/jasper-da-com/openapi/jasper-da-com-usage-api-openapi.yml
- filename: jasper-da-com-users-api-openapi.yml
  format: yaml
  label: Jasper Users API
  slug: jasper-da-com-users-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/jasper-da-com/openapi/jasper-da-com-users-api-openapi.yml
- filename: jasper-da-com-voices-api-openapi.yml
  format: yaml
  label: Jasper Voices API
  slug: jasper-da-com-voices-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/jasper-da-com/openapi/jasper-da-com-voices-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: jasper.ai
  spf: true
hosts:
- cert_expires: Jan  9 12:55:02 2027 GMT
  host: www.jasper.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Jasper Da Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Jasper, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Jasper
provider_slug: jasper-da-com
slug: jasper-da-com-domain-security
source_filename: jasper-da-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-23'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.jasper.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  9 12:55:02 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: jasper.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/jasper-da-com/security/jasper-da-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- AI
- Marketing
- Automation
- Content
- Platform
- Company
---
