---
api_specs:
- filename: voxco-aicoder-api-openapi.yml
  format: yaml
  label: Voxco AICoder API
  slug: voxco-aicoder-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/voxco/refs/heads/main/openapi/voxco-aicoder-api-openapi.yml
- filename: voxco-codebooks-api-openapi.yml
  format: yaml
  label: Voxco Codebooks API
  slug: voxco-codebooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/voxco/refs/heads/main/openapi/voxco-codebooks-api-openapi.yml
- filename: voxco-companies-api-openapi.yml
  format: yaml
  label: Voxco Companies API
  slug: voxco-companies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/voxco/refs/heads/main/openapi/voxco-companies-api-openapi.yml
- filename: voxco-exports-api-openapi.yml
  format: yaml
  label: Voxco Exports API
  slug: voxco-exports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/voxco/refs/heads/main/openapi/voxco-exports-api-openapi.yml
- filename: voxco-languages-api-openapi.yml
  format: yaml
  label: Voxco Languages API
  slug: voxco-languages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/voxco/refs/heads/main/openapi/voxco-languages-api-openapi.yml
- filename: voxco-questions-api-openapi.yml
  format: yaml
  label: Voxco Questions API
  slug: voxco-questions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/voxco/refs/heads/main/openapi/voxco-questions-api-openapi.yml
- filename: voxco-responses-api-openapi.yml
  format: yaml
  label: Voxco Responses API
  slug: voxco-responses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/voxco/refs/heads/main/openapi/voxco-responses-api-openapi.yml
- filename: voxco-sessions-api-openapi.yml
  format: yaml
  label: Voxco Sessions API
  slug: voxco-sessions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/voxco/refs/heads/main/openapi/voxco-sessions-api-openapi.yml
- filename: voxco-studies-api-openapi.yml
  format: yaml
  label: Voxco Studies API
  slug: voxco-studies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/voxco/refs/heads/main/openapi/voxco-studies-api-openapi.yml
- filename: voxco-studyrespondents-api-openapi.yml
  format: yaml
  label: Voxco StudyRespondents API
  slug: voxco-studyrespondents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/voxco/refs/heads/main/openapi/voxco-studyrespondents-api-openapi.yml
- filename: voxco-users-api-openapi.yml
  format: yaml
  label: Voxco Users API
  slug: voxco-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/voxco/refs/heads/main/openapi/voxco-users-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: voxco.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: goascribe.com
  spf: true
hosts:
- cert_expires: Aug 16 00:00:36 2026 GMT
  host: www.voxco.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 19 23:59:59 2026 GMT
  host: na1.voxco.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  1 23:59:59 2026 GMT
  host: webservices.goascribe.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Voxco Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Voxco, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Voxco
provider_slug: voxco
slug: voxco-domain-security
source_filename: voxco-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.voxco.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 16 00:00:36 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: na1.voxco.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 19 23:59:59 2026 GMT\n  hsts: false\n- host: webservices.goascribe.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  1 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: voxco.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: goascribe.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/voxco/refs/heads/main/security/voxco-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Survey Software
- Market Research
- CATI
- Omnichannel
- Text Analytics
- Data Collection
- Panel Management
---
