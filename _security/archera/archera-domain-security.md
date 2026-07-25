---
api_specs:
- filename: archera-commitment-plans-api-openapi.yml
  format: yaml
  label: Archera Commitment Plans API
  slug: archera-commitment-plans-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/archera/refs/heads/main/openapi/archera-commitment-plans-api-openapi.yml
- filename: archera-commitments-api-openapi.yml
  format: yaml
  label: Archera Commitments API
  slug: archera-commitments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/archera/refs/heads/main/openapi/archera-commitments-api-openapi.yml
- filename: archera-exchanges-api-openapi.yml
  format: yaml
  label: Archera Exchanges API
  slug: archera-exchanges-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/archera/refs/heads/main/openapi/archera-exchanges-api-openapi.yml
- filename: archera-metrics-api-openapi.yml
  format: yaml
  label: Archera Metrics API
  slug: archera-metrics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/archera/refs/heads/main/openapi/archera-metrics-api-openapi.yml
- filename: archera-oauth-api-openapi.yml
  format: yaml
  label: Archera OAuth API
  slug: archera-oauth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/archera/refs/heads/main/openapi/archera-oauth-api-openapi.yml
- filename: archera-orgs-api-openapi.yml
  format: yaml
  label: Archera Orgs API
  slug: archera-orgs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/archera/refs/heads/main/openapi/archera-orgs-api-openapi.yml
- filename: archera-resources-api-openapi.yml
  format: yaml
  label: Archera Resources API
  slug: archera-resources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/archera/refs/heads/main/openapi/archera-resources-api-openapi.yml
- filename: archera-uploads-api-openapi.yml
  format: yaml
  label: Archera Uploads API
  slug: archera-uploads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/archera/refs/heads/main/openapi/archera-uploads-api-openapi.yml
- filename: archera-well-known-api-openapi.yml
  format: yaml
  label: Archera Well-Known API
  slug: archera-well-known-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/archera/refs/heads/main/openapi/archera-well-known-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: archera.ai
  spf: true
hosts:
- cert_expires: Sep 23 23:11:03 2026 GMT
  host: archera.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 23 21:44:57 2026 GMT
  host: docs.archera.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  4 23:59:59 2026 GMT
  host: api.archera.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Archera Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Archera, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Archera
provider_slug: archera
slug: archera-domain-security
source_filename: archera-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: archera.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 23:11:03 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.archera.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 23 21:44:57 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.archera.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  4 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: archera.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/archera/refs/heads/main/security/archera-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Developer Tools
- FinOps
- Cloud Cost Management
- Cloud Commitments
- Cost Optimization
- MCP
- Azure
- Google Cloud
---
