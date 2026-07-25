---
api_specs:
- filename: biolevate-agent-api-openapi.yml
  format: yaml
  label: Biolevate Agent API
  slug: biolevate-agent-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/biolevate/refs/heads/main/openapi/biolevate-agent-api-openapi.yml
- filename: biolevate-collections-api-openapi.yml
  format: yaml
  label: Biolevate Collections API
  slug: biolevate-collections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/biolevate/refs/heads/main/openapi/biolevate-collections-api-openapi.yml
- filename: biolevate-extraction-api-openapi.yml
  format: yaml
  label: Biolevate Extraction API
  slug: biolevate-extraction-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/biolevate/refs/heads/main/openapi/biolevate-extraction-api-openapi.yml
- filename: biolevate-files-api-openapi.yml
  format: yaml
  label: Biolevate Files API
  slug: biolevate-files-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/biolevate/refs/heads/main/openapi/biolevate-files-api-openapi.yml
- filename: biolevate-find-similar-files-api-openapi.yml
  format: yaml
  label: Biolevate Find similar files API
  slug: biolevate-find-similar-files-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/biolevate/refs/heads/main/openapi/biolevate-find-similar-files-api-openapi.yml
- filename: biolevate-multi-dimensional-extraction-api-openapi.yml
  format: yaml
  label: Biolevate Multi-Dimensional Extraction API
  slug: biolevate-multi-dimensional-extraction-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/biolevate/refs/heads/main/openapi/biolevate-multi-dimensional-extraction-api-openapi.yml
- filename: biolevate-provider-items-api-openapi.yml
  format: yaml
  label: Biolevate Provider Items API
  slug: biolevate-provider-items-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/biolevate/refs/heads/main/openapi/biolevate-provider-items-api-openapi.yml
- filename: biolevate-providers-api-openapi.yml
  format: yaml
  label: Biolevate Providers API
  slug: biolevate-providers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/biolevate/refs/heads/main/openapi/biolevate-providers-api-openapi.yml
- filename: biolevate-question-answering-api-openapi.yml
  format: yaml
  label: Biolevate Question Answering API
  slug: biolevate-question-answering-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/biolevate/refs/heads/main/openapi/biolevate-question-answering-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: biolevate.com
  spf: true
hosts:
- cert_expires: Sep 10 00:14:32 2026 GMT
  host: www.biolevate.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Biolevate Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Biolevate, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Biolevate
provider_slug: biolevate
slug: biolevate-domain-security
source_filename: biolevate-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.biolevate.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 10 00:14:32 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: biolevate.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/biolevate/refs/heads/main/security/biolevate-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Artificial Intelligence
- Life Sciences
- Regulatory Affairs
- Document Intelligence
- Knowledge Management
- Pharmaceuticals
- Machine Learning
---
