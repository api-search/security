---
api_specs:
- filename: gtm-agent-api-v1-api-openapi.yml
  format: yaml
  label: Agent API
  slug: agent-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gtm/openapi/gtm-agent-api-v1-api-openapi.yml
- filename: gtm-copilot-api-v1-api-openapi.yml
  format: yaml
  label: Copilot API
  slug: copilot-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gtm/openapi/gtm-copilot-api-v1-api-openapi.yml
- filename: gtm-data-api-v1-api-openapi.yml
  format: yaml
  label: Data API
  slug: data-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gtm/openapi/gtm-data-api-v1-api-openapi.yml
- filename: gtm-data-quality-api-v1-api-openapi.yml
  format: yaml
  label: Data Quality API
  slug: data-quality-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gtm/openapi/gtm-data-quality-api-v1-api-openapi.yml
- filename: gtm-studio-api-v1-api-openapi.yml
  format: yaml
  label: Studio API
  slug: studio-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gtm/openapi/gtm-studio-api-v1-api-openapi.yml
- filename: gtm-marketing-api-v1-api-openapi.yml
  format: yaml
  label: Marketing API
  slug: marketing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gtm/openapi/gtm-marketing-api-v1-api-openapi.yml
- filename: gtm-platform-api-v1-api-openapi.yml
  format: yaml
  label: Platform API
  slug: platform-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gtm/openapi/gtm-platform-api-v1-api-openapi.yml
- filename: gtm-vertical-datasets-api-v1-api-openapi.yml
  format: yaml
  label: Vertical Datasets API
  slug: vertical-datasets-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gtm/openapi/gtm-vertical-datasets-api-v1-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: gtm.ai
  spf: true
hosts:
- cert_expires: Dec 24 15:34:46 2026 GMT
  host: gtm.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Gtm Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ZoomInfo, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: ZoomInfo
provider_slug: gtm
slug: gtm-domain-security
source_filename: gtm-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: gtm.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 24 15:34:46 2026 GMT\n  hsts: false\ndomains:\n- domain: gtm.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/gtm/security/gtm-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- B2B
- Data
- Sales
---
