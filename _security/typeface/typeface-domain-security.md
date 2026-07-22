---
api_specs:
- filename: typeface-api-openapi.json
  format: json
  label: Typeface API
  slug: typeface-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/typeface/refs/heads/main/openapi/typeface-api-openapi.json
- filename: typeface-content-workflow-openapi.json
  format: json
  label: Typeface Content Workflow API
  slug: typeface-content-workflow-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/typeface/refs/heads/main/openapi/typeface-content-workflow-openapi.json
- filename: typeface-documents-search-openapi.json
  format: json
  label: Typeface Documents Search API
  slug: typeface-documents-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/typeface/refs/heads/main/openapi/typeface-documents-search-openapi.json
- filename: typeface-team-users-openapi.json
  format: json
  label: Typeface Team Users API
  slug: typeface-team-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/typeface/refs/heads/main/openapi/typeface-team-users-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: typeface.ai
  spf: true
hosts:
- cert_expires: Oct  9 01:18:28 2026 GMT
  host: www.typeface.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 16 05:51:39 2026 GMT
  host: api-us.typeface.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Typeface Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Typeface, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Typeface
provider_slug: typeface
slug: typeface-domain-security
source_filename: typeface-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.typeface.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  9 01:18:28 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api-us.typeface.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 16 05:51:39 2026 GMT\n  hsts: null\ndomains:\n- domain: typeface.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/typeface/refs/heads/main/security/typeface-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Ai
- Artificial Intelligence
- Content Generation
- Marketing
- Agents
- Generative AI
- Brand Management
- Enterprise
---
