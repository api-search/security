---
api_specs:
- filename: alderinvoices-com-drafts-api-openapi.yml
  format: yaml
  label: Alder Drafts API
  slug: alderinvoices-com-drafts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/alderinvoices-com/openapi/alderinvoices-com-drafts-api-openapi.yml
- filename: alderinvoices-com-pdf-api-openapi.yml
  format: yaml
  label: Alder PDF API
  slug: alderinvoices-com-pdf-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/alderinvoices-com/openapi/alderinvoices-com-pdf-api-openapi.yml
- filename: alderinvoices-com-template-drafts-api-openapi.yml
  format: yaml
  label: Alder Template Drafts API
  slug: alderinvoices-com-template-drafts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/alderinvoices-com/openapi/alderinvoices-com-template-drafts-api-openapi.yml
- filename: alderinvoices-com-templates-api-openapi.yml
  format: yaml
  label: Alder Templates API
  slug: alderinvoices-com-templates-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/alderinvoices-com/openapi/alderinvoices-com-templates-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: alderinvoices.com
  spf: true
hosts:
- cert_expires: Dec 26 00:35:30 2026 GMT
  host: alderinvoices.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Alder Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Alder, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Alder
provider_slug: alderinvoices-com
slug: alderinvoices-com-domain-security
source_filename: alderinvoices-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: alderinvoices.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 26 00:35:30 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: alderinvoices.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/alderinvoices-com/security/alderinvoices-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Invoices
- Finance
- PDF
- Free
- MCP
---
