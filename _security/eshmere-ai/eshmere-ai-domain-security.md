---
api_specs:
- filename: eshmere-ai-drafting-api-openapi.yml
  format: yaml
  label: Eshmere Ltd Drafting API
  slug: eshmere-ai-drafting-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/eshmere-ai/openapi/eshmere-ai-drafting-api-openapi.yml
- filename: eshmere-ai-pipeline-api-openapi.yml
  format: yaml
  label: Eshmere Ltd Pipeline API
  slug: eshmere-ai-pipeline-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/eshmere-ai/openapi/eshmere-ai-pipeline-api-openapi.yml
- filename: eshmere-ai-read-api-openapi.yml
  format: yaml
  label: Eshmere Ltd Read API
  slug: eshmere-ai-read-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/eshmere-ai/openapi/eshmere-ai-read-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: eshmere.ai
  spf: true
hosts:
- cert_expires: Dec 22 23:23:22 2026 GMT
  host: www.eshmere.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Eshmere Ltd Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Eshmere Ltd, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Eshmere Ltd
provider_slug: eshmere-ai
slug: eshmere-ai-domain-security
source_filename: eshmere-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-07'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.eshmere.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 22 23:23:22 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: eshmere.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/eshmere-ai/security/eshmere-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Artificial Intelligence
- Public Procurement
- Real Estate
- Automation
- Software-as-a-Service
---
