---
api_specs:
- filename: yoodli-multi-org-management-api-openapi.yml
  format: yaml
  label: Yoodli Multi Org Management API
  slug: yoodli-multi-org-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yoodli/refs/heads/main/openapi/yoodli-multi-org-management-api-openapi.yml
- filename: yoodli-organization-user-management-api-openapi.yml
  format: yaml
  label: Yoodli Organization User Management API
  slug: yoodli-organization-user-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yoodli/refs/heads/main/openapi/yoodli-organization-user-management-api-openapi.yml
- filename: yoodli-speech-api-openapi.yml
  format: yaml
  label: Yoodli Speech API
  slug: yoodli-speech-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yoodli/refs/heads/main/openapi/yoodli-speech-api-openapi.yml
- filename: yoodli-user-group-management-api-openapi.yml
  format: yaml
  label: Yoodli User Group Management API
  slug: yoodli-user-group-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yoodli/refs/heads/main/openapi/yoodli-user-group-management-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: yoodli.ai
  spf: true
hosts:
- cert_expires: Nov  9 03:56:39 2026 GMT
  host: yoodli.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 28 16:46:14 2026 GMT
  host: developers.yoodli.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  9 03:56:39 2026 GMT
  host: app.yoodli.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Yoodli Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Yoodli, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Yoodli
provider_slug: yoodli
slug: yoodli-domain-security
source_filename: yoodli-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: yoodli.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  9 03:56:39 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developers.yoodli.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 28 16:46:14 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: app.yoodli.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  9 03:56:39 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: yoodli.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/yoodli/refs/heads/main/security/yoodli-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Artificial Intelligence
- Communications
- Coaching
- Learning and Development
- Sales Enablement
- Speech Analysis
- Human Resources
- Enterprise Software
- Software-as-a-Service
- Identity Management
---
