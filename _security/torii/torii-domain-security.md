---
api_specs:
- filename: torii-apps-api-openapi.yml
  format: yaml
  label: Torii Apps API
  slug: torii-apps-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/torii/refs/heads/main/openapi/torii-apps-api-openapi.yml
- filename: torii-audit-api-openapi.yml
  format: yaml
  label: Torii Audit API
  slug: torii-audit-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/torii/refs/heads/main/openapi/torii-audit-api-openapi.yml
- filename: torii-contracts-api-openapi.yml
  format: yaml
  label: Torii Contracts API
  slug: torii-contracts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/torii/refs/heads/main/openapi/torii-contracts-api-openapi.yml
- filename: torii-files-api-openapi.yml
  format: yaml
  label: Torii Files API
  slug: torii-files-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/torii/refs/heads/main/openapi/torii-files-api-openapi.yml
- filename: torii-metadata-api-openapi.yml
  format: yaml
  label: Torii Metadata API
  slug: torii-metadata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/torii/refs/heads/main/openapi/torii-metadata-api-openapi.yml
- filename: torii-parsings-api-openapi.yml
  format: yaml
  label: Torii Parsings API
  slug: torii-parsings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/torii/refs/heads/main/openapi/torii-parsings-api-openapi.yml
- filename: torii-scim-api-openapi.yml
  format: yaml
  label: Torii SCIM API
  slug: torii-scim-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/torii/refs/heads/main/openapi/torii-scim-api-openapi.yml
- filename: torii-services-api-openapi.yml
  format: yaml
  label: Torii Services API
  slug: torii-services-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/torii/refs/heads/main/openapi/torii-services-api-openapi.yml
- filename: torii-users-api-openapi.yml
  format: yaml
  label: Torii Users API
  slug: torii-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/torii/refs/heads/main/openapi/torii-users-api-openapi.yml
- filename: torii-workflows-api-openapi.yml
  format: yaml
  label: Torii Workflows API
  slug: torii-workflows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/torii/refs/heads/main/openapi/torii-workflows-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: toriihq.com
  spf: true
hosts:
- cert_expires: Sep 16 01:48:11 2026 GMT
  host: www.toriihq.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 15 06:50:47 2026 GMT
  host: developers.toriihq.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar  2 23:59:59 2027 GMT
  host: api.toriihq.com
  hsts: true
  hsts_max_age: 15768000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Torii Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Torii, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Torii
provider_slug: torii
slug: torii-domain-security
source_filename: torii-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.toriihq.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 01:48:11 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: developers.toriihq.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 06:50:47 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.toriihq.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar  2 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 15768000\ndomains:\n- domain: toriihq.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/torii/refs/heads/main/security/torii-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Application
- Compliance
- Cost Optimization
- Governance
- IT Management
- SaaS Management
---
