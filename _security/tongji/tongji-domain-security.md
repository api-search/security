---
api_specs:
- filename: tongji-ai-services-api-openapi.yml
  format: yaml
  label: Tongji University AI Services API
  slug: tongji-ai-services-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tongji/refs/heads/main/openapi/tongji-ai-services-api-openapi.yml
- filename: tongji-assets-and-procurement-api-openapi.yml
  format: yaml
  label: Tongji University Assets and Procurement API
  slug: tongji-assets-and-procurement-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tongji/refs/heads/main/openapi/tongji-assets-and-procurement-api-openapi.yml
- filename: tongji-education-data-verification-api-openapi.yml
  format: yaml
  label: Tongji University Education Data Verification API
  slug: tongji-education-data-verification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tongji/refs/heads/main/openapi/tongji-education-data-verification-api-openapi.yml
- filename: tongji-library-api-openapi.yml
  format: yaml
  label: Tongji University Library API
  slug: tongji-library-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tongji/refs/heads/main/openapi/tongji-library-api-openapi.yml
- filename: tongji-reference-metadata-api-openapi.yml
  format: yaml
  label: Tongji University Reference Metadata API
  slug: tongji-reference-metadata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tongji/refs/heads/main/openapi/tongji-reference-metadata-api-openapi.yml
- filename: tongji-research-api-openapi.yml
  format: yaml
  label: Tongji University Research API
  slug: tongji-research-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tongji/refs/heads/main/openapi/tongji-research-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: tongji.edu.cn
  spf: true
hosts:
- cert_expires: Oct 31 11:59:59 2026 GMT
  host: www.tongji.edu.cn
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 31 11:59:59 2026 GMT
  host: en.tongji.edu.cn
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 31 11:59:59 2026 GMT
  host: api.tongji.edu.cn
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Tongji Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Tongji University, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Tongji University
provider_slug: tongji
slug: tongji-domain-security
source_filename: tongji-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.tongji.edu.cn\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 31 11:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: en.tongji.edu.cn\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 31 11:59:59 2026 GMT\n  hsts: false\n- host: api.tongji.edu.cn\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 31 11:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: tongji.edu.cn\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tongji/refs/heads/main/security/tongji-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- University
- Higher Education
- Education
- China
- Shanghai
- Double First-Class
- Open Platform
- Campus Data
- Identity Federation
- Research Data
- Library
- Course Catalog
- Reference Data
---
