---
api_specs:
- filename: qualio-audit-trail-api-openapi.yml
  format: yaml
  label: Qualio Audit Trail API
  slug: qualio-audit-trail-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qualio/refs/heads/main/openapi/qualio-audit-trail-api-openapi.yml
- filename: qualio-change-management-api-openapi.yml
  format: yaml
  label: Qualio Change Management API
  slug: qualio-change-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qualio/refs/heads/main/openapi/qualio-change-management-api-openapi.yml
- filename: qualio-compliance-intelligence-api-openapi.yml
  format: yaml
  label: Qualio Compliance Intelligence API
  slug: qualio-compliance-intelligence-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qualio/refs/heads/main/openapi/qualio-compliance-intelligence-api-openapi.yml
- filename: qualio-design-controls-api-openapi.yml
  format: yaml
  label: Qualio Design Controls API
  slug: qualio-design-controls-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qualio/refs/heads/main/openapi/qualio-design-controls-api-openapi.yml
- filename: qualio-documents-api-openapi.yml
  format: yaml
  label: Qualio Documents API
  slug: qualio-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qualio/refs/heads/main/openapi/qualio-documents-api-openapi.yml
- filename: qualio-events-api-openapi.yml
  format: yaml
  label: Qualio Events API
  slug: qualio-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qualio/refs/heads/main/openapi/qualio-events-api-openapi.yml
- filename: qualio-resource-library-api-openapi.yml
  format: yaml
  label: Qualio Resource Library API
  slug: qualio-resource-library-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qualio/refs/heads/main/openapi/qualio-resource-library-api-openapi.yml
- filename: qualio-suppliers-api-openapi.yml
  format: yaml
  label: Qualio Suppliers API
  slug: qualio-suppliers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qualio/refs/heads/main/openapi/qualio-suppliers-api-openapi.yml
- filename: qualio-tags-api-openapi.yml
  format: yaml
  label: Qualio Tags API
  slug: qualio-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qualio/refs/heads/main/openapi/qualio-tags-api-openapi.yml
- filename: qualio-training-api-openapi.yml
  format: yaml
  label: Qualio Training API
  slug: qualio-training-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qualio/refs/heads/main/openapi/qualio-training-api-openapi.yml
- filename: qualio-user-management-api-openapi.yml
  format: yaml
  label: Qualio User Management API
  slug: qualio-user-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qualio/refs/heads/main/openapi/qualio-user-management-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: qualio.com
  spf: true
hosts:
- cert_expires: Sep 13 03:58:02 2026 GMT
  host: qualio.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Qualio Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Qualio, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Qualio
provider_slug: qualio
slug: qualio-domain-security
source_filename: qualio-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: qualio.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 03:58:02 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: qualio.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/qualio/refs/heads/main/security/qualio-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Quality Management
- Life Sciences
- Compliance
- Document Control
- QMS
- Regulatory
- Medical Devices
---
