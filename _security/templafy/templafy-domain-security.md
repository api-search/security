---
api_specs:
- filename: templafy-datasourcefields-api-openapi.yml
  format: yaml
  label: Templafy DataSourceFields API
  slug: templafy-datasourcefields-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/templafy/refs/heads/main/openapi/templafy-datasourcefields-api-openapi.yml
- filename: templafy-datasourceitemfields-api-openapi.yml
  format: yaml
  label: Templafy DataSourceItemFields API
  slug: templafy-datasourceitemfields-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/templafy/refs/heads/main/openapi/templafy-datasourceitemfields-api-openapi.yml
- filename: templafy-datasourceitems-api-openapi.yml
  format: yaml
  label: Templafy DataSourceItems API
  slug: templafy-datasourceitems-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/templafy/refs/heads/main/openapi/templafy-datasourceitems-api-openapi.yml
- filename: templafy-datasources-api-openapi.yml
  format: yaml
  label: Templafy DataSources API
  slug: templafy-datasources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/templafy/refs/heads/main/openapi/templafy-datasources-api-openapi.yml
- filename: templafy-documents-api-openapi.yml
  format: yaml
  label: Templafy Documents API
  slug: templafy-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/templafy/refs/heads/main/openapi/templafy-documents-api-openapi.yml
- filename: templafy-emailelements-api-openapi.yml
  format: yaml
  label: Templafy EmailElements API
  slug: templafy-emailelements-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/templafy/refs/heads/main/openapi/templafy-emailelements-api-openapi.yml
- filename: templafy-folders-api-openapi.yml
  format: yaml
  label: Templafy Folders API
  slug: templafy-folders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/templafy/refs/heads/main/openapi/templafy-folders-api-openapi.yml
- filename: templafy-images-api-openapi.yml
  format: yaml
  label: Templafy Images API
  slug: templafy-images-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/templafy/refs/heads/main/openapi/templafy-images-api-openapi.yml
- filename: templafy-libraries-api-openapi.yml
  format: yaml
  label: Templafy Libraries API
  slug: templafy-libraries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/templafy/refs/heads/main/openapi/templafy-libraries-api-openapi.yml
- filename: templafy-links-api-openapi.yml
  format: yaml
  label: Templafy Links API
  slug: templafy-links-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/templafy/refs/heads/main/openapi/templafy-links-api-openapi.yml
- filename: templafy-pdfs-api-openapi.yml
  format: yaml
  label: Templafy Pdfs API
  slug: templafy-pdfs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/templafy/refs/heads/main/openapi/templafy-pdfs-api-openapi.yml
- filename: templafy-presentations-api-openapi.yml
  format: yaml
  label: Templafy Presentations API
  slug: templafy-presentations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/templafy/refs/heads/main/openapi/templafy-presentations-api-openapi.yml
- filename: templafy-slideelements-api-openapi.yml
  format: yaml
  label: Templafy SlideElements API
  slug: templafy-slideelements-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/templafy/refs/heads/main/openapi/templafy-slideelements-api-openapi.yml
- filename: templafy-slides-api-openapi.yml
  format: yaml
  label: Templafy Slides API
  slug: templafy-slides-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/templafy/refs/heads/main/openapi/templafy-slides-api-openapi.yml
- filename: templafy-spaces-api-openapi.yml
  format: yaml
  label: Templafy Spaces API
  slug: templafy-spaces-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/templafy/refs/heads/main/openapi/templafy-spaces-api-openapi.yml
- filename: templafy-spreadsheets-api-openapi.yml
  format: yaml
  label: Templafy Spreadsheets API
  slug: templafy-spreadsheets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/templafy/refs/heads/main/openapi/templafy-spreadsheets-api-openapi.yml
- filename: templafy-textelements-api-openapi.yml
  format: yaml
  label: Templafy TextElements API
  slug: templafy-textelements-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/templafy/refs/heads/main/openapi/templafy-textelements-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: templafy.com
  spf: true
hosts:
- cert_expires: Sep 14 19:50:53 2026 GMT
  host: www.templafy.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Templafy Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Templafy, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Templafy
provider_slug: templafy
slug: templafy-domain-security
source_filename: templafy-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.templafy.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 19:50:53 2026 GMT\n  hsts: false\ndomains:\n- domain: templafy.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/templafy/refs/heads/main/security/templafy-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Document Generation
- Templates
- Content Management
- Digital Asset Management
- Document Automation
- Productivity
- Enterprise
- Software-as-a-Service
---
